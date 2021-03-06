# 🐰

Barebones **vanilla** boilerplate. 
Built to be able to write simple pages that aren't necesarily single page apps nor require the scaffolding of a Static Site Generator like Next, Gatsby or Vuepress.

### Defaults
- **Babel 7** (`preset-env` set to ">2%, last 1 edge version, last 2 safari version, not ie 11, not op_mini all").
- **PostCSS** (CSS Modules + CSSNano)

### Entries
On the webpack configuration, each entry has it's own html file (about.js needs about.html). 
If you add a entry, make sure to add it's corresponding .html file. Other files under the public folder will be copied over.

### Hashing
There is no asset hashing to make serving the built folder as simple as possible. If you want to enable you just have to add `[hash:8]` to the filenames of the outputted / copied files.

### How to run locally
- `yarn install`
- `yarn start`

### Build for production
- `yarn build` -> Will output a build folder

### Linting
**ESLint & Prettier** (Using AirBnB defaults)
- `yarn lint` -> Will lint all code under `src` folder.
