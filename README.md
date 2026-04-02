# 🌳 AVL Tree Visualizer

An interactive, browser-based AVL (Adelson-Velsky and Landis) self-balancing binary search tree visualizer built with pure HTML, CSS, and JavaScript — no dependencies required.

---

## 📸 Features

- **Insert nodes** — single value or multiple space/comma-separated values
- **Delete nodes** — removes a value and rebalances the tree automatically
- **Random tree** — generates a random 7-node AVL tree instantly
- **Reset** — clears the entire tree
- **Balancing info toggle** — shows height (`h`) and balance factor (`bf`) inside each node
- **Tree traversals** — Inorder, Preorder, Postorder, and Level Order
- **Dark / Light theme** — toggle between themes with one click
- **Color-coded nodes** — each node gets a unique random HSL color for easy visual distinction

---

## 🚀 Getting Started

No installation or build step needed. Just open the file in any modern browser.

```bash
# Clone or download the project
git clone https://github.com/your-username/avl-tree-visualizer.git

# Open in browser
open index.html
```

Or simply double-click `index.html` to launch it.

---

## 🛠️ Usage

| Action | How To |
|---|---|
| Insert node(s) | Type numbers (e.g. `10 20 30`) → click **Insert** |
| Delete a node | Type a number → click **Delete** |
| Random tree | Click **Random** |
| Clear tree | Click **Reset** |
| Show h & bf | Check **Show Balancing Info** |
| Traversals | Click **Inorder / Preorder / Postorder / Level Order** |
| Toggle theme | Click **Toggle Theme** |

---

## ⚙️ How AVL Balancing Works

An AVL tree maintains the **balance factor** (BF) of every node:

```
BF = height(left subtree) − height(right subtree)
```

If BF goes outside the range **[-1, 1]**, a rotation is triggered:

| Case | Condition | Fix |
|---|---|---|
| Left-Left | BF > 1, key < left child | Right Rotate |
| Right-Right | BF < -1, key > right child | Left Rotate |
| Left-Right | BF > 1, key > left child | Left Rotate + Right Rotate |
| Right-Left | BF < -1, key < right child | Right Rotate + Left Rotate |

---

## 📁 Project Structure

```
avl-tree-visualizer/
└── index.html       # All logic, styles, and SVG rendering in one file
```

---

## 🧰 Tech Stack

- **HTML5** — structure and SVG rendering
- **CSS3** — theming with CSS variables (light/dark mode)
- **Vanilla JavaScript** — AVL tree logic and DOM manipulation
- **SVG** — dynamic tree drawing with lines and circles

---

## 🤝 Contributing

Pull requests are welcome! Feel free to open an issue for bugs or feature suggestions.

---
