# 🦀 Learning Rust as a Pythonista 🐍

**A daily journey to learn Rust, with Python side-by-side comparisons.**  
*Because sometimes you need to see it in Python first to "get" Rust!*

---

## 👋 Welcome, Python Developers!

This repository documents my daily progress learning Rust, focusing on **bridging the gap between Python and Rust**. If you’re coming from Python (like me!), you’ll find:  
- **Rust concepts explained with Python analogies**  
- **Side-by-side code snippets** (Python vs. Rust)  
- **Notes on Rust’s quirks** (like ownership) vs. Python’s flexibility  
- Why Rust is worth learning for data/backend tasks (spoiler: speed + safety 💥)

---

## 🗂️ Repository Structure

rust-learning-journey/
├── daily-progress/         # Daily folders (day-01, day-02, ...)
│   ├── day-01-ownership/   # Example: Ownership in Rust vs. Python
│   │   ├── notes.md        # Theory + Python comparisons
│   │   ├── code/           # Rust code with Python equivalents
│   │   └── README.md       # Daily summary + "Aha!" moments
├── projects/               # Mini-projects (e.g., CLI tools, data parsers)
├── python-vs-rust/         # Key syntax differences cheat sheet
└── resources.md            # Curated guides for Python devs learning Rust

---
## 🚀 How I’m Learning

### 1. **Theory First (But with Python Lens)**
- Example: When learning Rust’s `Result` type, I compare it to Python’s `try/except`.  
- Notes include: *“In Python, I’d just raise an error. In Rust, I have to handle it explicitly. 😅”*

### 2. **Code with Dual Examples**
Every Rust snippet comes with a Python equivalent. For example:

**Python (Mutable by default):**
```python
x = [1, 2, 3]
y = x  # Both x and y point to the same list
y.append(4)
print(x)  # [1, 2, 3, 4]
```

**Rust (Ownership rules!):**
```rust
fn main() {
    let x = vec![1, 2, 3];
    let y = x;  // Ownership moved to y – x is now invalid!
    // println!("{:?}", x);  ← This would fail!
    println!("{:?}", y);  // [1, 2, 3]
}
```

### 3. **Weekly Projects**
Building small tools in **both languages** to compare:
- Performance (Rust’s speed vs. Python’s ease)
- Error handling patterns
- Memory usage differences

---

## 📆 Progress Log

| Day | Topic                     | Rust vs. Python Takeaways          |
|-----|---------------------------|-------------------------------------|
| 01  | Variables & Ownership     | “Rust’s `let` is like Python’s `=`, but with prison rules.” 🚔 |
| 02  | Error Handling            | “Python: ‘YOLO’ exceptions. Rust: ‘Prove you handled it’.” 🔍 |
| 03  | Structs vs. Classes       | “Rust structs: like Python dataclasses but less magical.” 🧙 |
| ... |                           |                                     |

*(I’ll update this table daily!)*

---

## 🔑 Quick Syntax Comparison

| Concept          | Python Example             | Rust Example                     |
|------------------|----------------------------|----------------------------------|
| **Lists/Arrays** | `nums = [1, 2, 3]`         | `let nums = vec![1, 2, 3];`      |
| **Loops**        | `for num in nums:`         | `for num in &nums { ... }`       |
| **Type Hints**   | `def add(a: int) -> int:`  | `fn add(a: i32) -> i32 { ... }`  |
| **Dictionaries** | `data = {"key": "value"}`  | `let data = HashMap::new();`     |

---

## ❓ FAQ (From One Python Dev to Another)

**Q: Why learn Rust if I know Python?**  
A: For tasks where Python is too slow (big data processing, systems tools) or unsafe (memory leaks). Rust is like Python’s strict but super-efficient cousin.

**Q: Is Rust’s borrow checker really that hard?**  
A: At first, yes. It’s like going from Python’s “no rules” party to Rust’s “security guard checking your ID 3 times”. But you’ll learn to love it!

**Q: Can I use Rust for data science?**  
A: Not directly (yet!), but libraries like [Polars](https://www.pola.rs/) (built in Rust) show its potential. Great for building high-performance data pipelines.

---

## 🤝 Contributing

Found a better way to explain a Rust concept to Python devs? **PRs welcome!** Let’s make this repo a friendly guide for:
- Adding more Python comparisons
- Fixing my "Rustacean-in-training" mistakes 😬
- Suggesting projects to build in both languages

---

## 📚 Resources I’m Using

- **The Rust Book**: [doc.rust-lang.org/book](https://doc.rust-lang.org/book/)  
- **Rust for Python Programmers**: [github.com/rochacbruno/rust-python](https://github.com/rochacbruno/rust-python)  
- **Why Rust?**: [whyrust.pl](https://whyrust.pl/)  

---

*Started on [Date]. Still fighting the borrow checker daily. 🛡️*  
**[Connect with me](https://your-linkedin/github)** | *License: MIT*

