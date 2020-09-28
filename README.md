# eclipse-che-devfiles

[Eclipse Che](https://www.eclipse.org/che/)で利用するworkspace設定ファイル群

---

## [simple-js.yaml](./simple-js.yaml)

- Javascript学習用リポジトリ
- 利用コンポーネント
  - [nginx-static](https://github.com/sakurai-lab-info/docker-images/tree/master/nginx-static)
    - [nginx](https://nginx.org/en/)で`/projects/`以下を公開するだけのコンポーネント
- commands:
  - start/stop/restart nginx
  - Configure nginx Web Server DocumentRoot
    - nginxの公開ディレクトリを`simple-js/`にする

### 使い方

- [開発環境](https://che-che.sakurai-lab.info)を開く
- `Workspaces`を開き、`Add Workspace`ボタンを押す
- `Devfile`欄の`URL of devfile`項目に当該devfileのURL(下記の通り)を貼る
  - `https://raw.githubusercontent.com/sakurai-lab-info/eclipse-che-devfiles/master/simple-js.yaml`
- 読み込まれたDevfileの一部を書き換える
  - `@@YOUR-REPOSITORY-URL@@`の部分を自分がforkしたリポジトリのURLに置き換える
  - 例: `https://github.com/自分のアカウント名/simple-js.git`
- 左下の`Create & Open`ボタンを押す
