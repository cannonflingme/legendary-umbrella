{
  "name": "github-readme-stats",
  "version": "1.0.0",
  "description": "Dynamically generate stats for your GitHub readme",
  "keywords": [
    "github-readme-stats",
    "readme-stats",
    "cards",
    "card-generator"
  ],
  "main": "src/index.js",
  "type": "module",
  "homepage": "https://github.com/anuraghazra/github-readme-stats",
  "bugs": {
    "url": "https://github.com/anuraghazra/github-readme-stats/issues"
  },
  "repository": {
    "type": "git",
    "url": "https://github.com/anuraghazra/github-readme-stats.git"
  },
  "scripts": {
    "test": "node --experimental-vm-modules node_modules/jest/bin/jest.js --coverage",
    "test:watch": "node --experimental-vm-modules node_modules/jest/bin/jest.js --watch",
    "test:update:snapshot": "node --experimental-vm-modules node_modules/jest/bin/jest.js -u",
    "test:e2e": "node --experimental-vm-modules node_modules/jest/bin/jest.js --config jest.e2e.config.js",
    "theme-readme-gen": "node scripts/generate-theme-doc",
    "preview-theme": "node scripts/preview-theme",
    "close-stale-theme-prs": "node scripts/close-stale-theme-prs",
    "generate-langs-json": "node scripts/generate-langs-json",
    "format": "prettier --write .",
    "format:check": "prettier --check .",
    "prepare": "husky",
    "lint": "npx eslint --max-warnings 0 \"./src/**/*.js\" \"./scripts/**/*.js\" \"./tests/**/*.js\" \"./api/**/*.js\" \"./themes/**/*.js\"",
    "bench": "node --experimental-vm-modules node_modules/jest/bin/jest.js --config jest.bench.config.js"
  },
  "author": "Anurag Hazra",
  "license": "MIT",
  "devDependencies": {
    "@actions/core": "^1.10.1",
    "@actions/github": "^6.0.0",
    "@testing-library/dom": "^10.1.0",
    "@testing-library/jest-dom": "^6.4.5",
    "@uppercod/css-to-object": "^1.1.1",
    "axios-mock-adapter": "^1.22.0",
    "color-contrast-checker": "^2.1.0",
    "eslint": "^8.57.0",
    "eslint-config-prettier": "^9.1.0",
    "hjson": "^3.2.2",
    "husky": "^9.0.11",
    "jest": "^29.7.0",
    "jest-bench": "^29.7.1",
    "jest-environment-jsdom": "^29.7.0",
    "js-yaml": "^4.1.0",
    "lint-staged": "^15.2.2",
    "lodash.snakecase": "^4.1.1",
    "parse-diff": "^0.11.1",
    "prettier": "^3.2.5"
  },
  "dependencies": {
    "axios": "^1.7.1",
    "dotenv": "^16.4.5",
    "emoji-name-map": "^1.2.8",
    "github-username-regex": "^1.0.0",
    "upgrade": "^1.1.0",
    "word-wrap": "^1.2.5"
  },
  "lint-staged": {
    "*.{js,css,md}": "prettier --write"
  },
  "engines": {
    "node": ">=18.0.0"
  }
}
