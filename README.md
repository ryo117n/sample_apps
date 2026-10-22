# Ruby on Railsチュートリアル: サンプルアプリケーション

これは以下に基づいたサンプル・アプリケーションです
[*Ruby on Railsチュートリアル:
実例を使ってRailsを学ぼう*](http://railstutorial.jp/)
[Michael Hartl](http://www.michaelhartl.com/)著

## Node.js for Rails assets

Use Node.js 22.23.4 for JavaScript asset compilation. The locked Uglifier and
CoffeeScript gems use ExecJS, which can select Node.js even when the application
has no npm dependencies. The `.node-version` and `.nvmrc` files select the fixed
October 2026 security release. With nvm, run `nvm install && nvm use` before
compiling assets and verify `node --version`.

Apply this runtime selection in any asset-build or deployment environment that
uses Node.js through ExecJS. Updating these files does not update an already
running deployment. Rails, Ruby and database versions are unchanged.
