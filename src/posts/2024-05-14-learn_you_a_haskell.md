---
author: "Benjamin Prevor"
authorTwitter: "@BenjaminPrevor"
desc: "a review of Learn You a Haskell for Great Good"
image: "./images/learn_you_a_haskell.jpg"
keywords: "book_review, haskell,"
lang: "en"
title: "Learn You a Haskell for Great Good!"
updated: "2024-05-09T12:00:00Z"
year: "2024"
---

"Learn You a Haskell for Great Good! A Beginner's Guide" by Miran Lipovača http://localhost:3000

<img
  alt="learn you a haskell for great good by Miran Lipovaca"
  src="./images/learn_you_a_haskell.jpg"
  height="200"
/>

I came into this book in a very specific context that gives it a softspot in my mind, for all intents and purposes

Haskell, for example:

```haskell
toSlug :: T.Text -> T.Text
toSlug =
  T.intercalate (T.singleton '-') . T.words . T.toLower . clean
```
