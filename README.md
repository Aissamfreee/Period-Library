## ⏳ clsPeriod Library

## 📌 Overview

`clsPeriod` is a C++ class that represents a time period defined by a start date and an end date.

It is built on top of `clsDate` and provides functionality for working with date ranges.

---

## 🚀 Features

* 📅 Define a period:

  * Start date
  * End date

* 🔄 Period comparison:

  * Check if two periods overlap

* 🖨️ Output:

  * Print period details

---

## 🛠️ Usage

```cpp
#include "clsPeriod.h"

int main() {
    clsDate start1(1, 1, 2024);
    clsDate end1(10, 1, 2024);

    clsDate start2(5, 1, 2024);
    clsDate end2(15, 1, 2024);

    clsPeriod p1(start1, end1);
    clsPeriod p2(start2, end2);

    if (clsPeriod::IsOverlapPeriods(p1, p2))
        cout << "Overlapping" << endl;
    else
        cout << "Not overlapping" << endl;

    return 0;
}
```

---

## 🧠 Design Notes

* Uses `clsDate` for all date operations
* Implements interval overlap logic

---

## ⚠️ Limitations

* No validation for invalid periods (start > end)
* Limited functionality (no duration or intersection)

---

## 📌 Future Improvements

* Add duration calculation
* Add intersection and merging
* Improve validation logic
