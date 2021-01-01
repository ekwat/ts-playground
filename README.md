# ts-playground
TypeScript + Node.js実行環境のテンプレート

## 実行環境と使用パッケージ
 - Node.js 14.15.0
 - npm 6.14.9
 - "typescript": "^4.1.3" `./node_modules/.bin/tsc --version`
 - "npm-run-all": "^4.1.5",
 - "rimraf": "^3.0.2",
 - "ts-node": "^9.1.1",
 - "ts-node-dev": "^1.1.1",
 
TypeScript -> JavaScript に変換
npm run build
生成されたJavaScriptを実行
npm run start
または
npm start
生成されたファイルを削除
npm run clean
---
ts-node-devでindex.tsの変更を検知するたびにプログラムを実行する
`npx ts-node-dev --respawn src/index.ts`
プロセスが一度で終了するプログアムはts-node-dev に --respawn オプションをつける
