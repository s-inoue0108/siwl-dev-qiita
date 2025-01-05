# SIWL.dev Qiita

This is the subtree of [@s-inoue0108/siwl-dev](https://github.com/s-inoue0108/siwl-dev).

- https://qiita.com/s-inoue0108

## Qiita CLI

Qiita CLI can be used in `/qiita/*`.

* [📘 How to use](https://qiita.com/Qiita/items/666e190490d0af90a92b)

## Export article from this blog

Automatically rewrite frontmatter and non-compliant syntax.

```bash
yarn run siwl ex -f <filename> -t qiita
```

### Push to parent repository with qiita repository

```bash
yarn run deploy --qiita
```

### Push only qiita repository

```bash
git subtree push --prefix=qiita qiita main
```

### Synchronize

```bash
git subtree pull --prefix=qiita --squash qiita main
yarn run deploy
```