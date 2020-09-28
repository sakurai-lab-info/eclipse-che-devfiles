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
    - nginxの公開

### 使い方

- [開発環境](https://che-che.sakurai-lab.info)を開く
- `Workspaces`を開き、`Add Workspace`ボタンを押す
- `Devfile`欄の`URL of devfile`項目に当該devfileのURL(下記の通り)を貼る
  - `https://raw.githubusercontent.com/sakurai-lab-info/eclipse-che-devfiles/master/simple-js.yaml`

