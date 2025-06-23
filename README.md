# Is-the-Score-Consistent

This C++ program is solving a problem that checks if a transformation or upgrade from one pair of values to another is **possible** under certain conditions.

### Breakdown of the Code:

#### 1. **Read Number of Test Cases**

```cpp
int T;
cin >> T;
```

* The program starts by reading an integer `T`, the number of test cases.

#### 2. **Loop Over Test Cases**

```cpp
while (T--) {
    int A, B, C, D;
    cin >> A >> B;
    cin >> C >> D;
```

* For each test case, it reads 4 integers:

  * `A`, `B` — the initial values
  * `C`, `D` — the target values

#### 3. **Check the Condition**

```cpp
if (C >= A && D >= B)
    cout << "POSSIBLE" << endl;
else
    cout << "IMPOSSIBLE" << endl;
```

* The program checks whether both `C` is **greater than or equal to** `A`, **and** `D` is greater than or equal to `B`.

  * If so, it prints `POSSIBLE`
  * Otherwise, it prints `IMPOSSIBLE`

### 🧠 Interpretation:

This logic suggests you can "upgrade" from `(A, B)` to `(C, D)` only if **both** values don’t decrease.

---

