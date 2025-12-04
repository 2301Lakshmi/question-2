---
marp: true
theme: custom-theme
paginate: true
paginate-placement: bottom-right
---

<!--
You can convert this using:
marp slides.md --html --theme custom-theme.css
marp slides.md --pdf
-->

# **Product Documentation Presentation**
### Author: 22f1000912@ds.study.iitm.ac.in

---

# **Overview**

- Modern Marp-based documentation  
- Version-controlled Markdown  
- Convertible to PDF / HTML / PPTX  
- Custom theme + styling  
- Background images  
- Math equations using KaTeX  

---

<!-- Custom background image slide -->
![bg](https://source.unsplash.com/1600x900/?technology,software)

# **Background Image Example**

This slide uses a full-screen background image via Marp `![bg]()` syntax.

---

# **Algorithmic Complexity**

We often express algorithmic cost using Big-O notation:

\[
T(n) = O(n \log n)
\]

Or more generally:

\[
T(n) = a n^2 + b n + c
\]

---

# **Sample Code Snippet**

```python
def binary_search(arr, target):
    low, high = 0, len(arr)-1
    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        if arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return -1
