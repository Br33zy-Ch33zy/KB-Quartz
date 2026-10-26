---
type: tool
category: web
tags:
  - tool
---
# Overview
Quartz is a framework, which allows to convert `.md` file-structures, like `obsidian` vaults to `html` files and build a website.
## How to setup
1. Install `node.js` and `npm`
2. Clone quartz-repo and install it 
```bash
git clone https://github.com/jackyzha0/quartz.git quartz
cd quartz
npm install
```
3. Initialize site with wizard:
```bash
npx quartz create
```
- A **template** (`default`, `obsidian`, `ttrpg`, `blog`) — pick the one that matches your use case. See [create > Templates](https://quartz.jzhao.xyz/cli/create#templates) for details on each.
- A **content strategy** — choose how to populate the `content/` folder:
    - **new**: Start with an empty folder
    - **copy**: Copy files from an existing folder (e.g. your Obsidian vault)
    - **symlink**: Link to an existing folder so changes sync automatically
- A **base URL** — the URL where your site will be deployed (e.g. `mysite.github.io/quartz`). Don’t include `https://`.
- A **link resolution** strategy — how to resolve internal links (`shortest`, `absolute`, or `relative`). Skipped for Obsidian and TTRPG templates.

4. Copy `.md` files to the folder `/content`
5. Install plugins:
```bash
   npx quartz plugin install --from-config
```


## Important Parameter
