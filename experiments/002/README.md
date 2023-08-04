- sub に peerDependencies があるとき、次の挙動になるか？
  - main で yarn を実行しても、peerDependencies の警告が出るだけでインストールはされない  
    → 正しい。unmet peer dependency という警告が出力される
- この状態で main 側で `node index.js` を行うとエラーが出るか？  
  → 出る
- main 側で `yarn add react` を行うとエラーは解消されるか？  
  → される。きちんと main 側の React が使われているようだ
