# C Hello World 範例學習紀錄

這個專案示範最簡單的 C 程式：輸出 `Hello, world!`。

## 1. 建立檔案

建立 `hello.c`：

```c
#include <stdio.h>

int main() {
    printf("Hello, world!\n");
    return 0;
}
```

## 2. 編譯程式

在終端機執行：

```bash
gcc hello.c -o hello
```

這會產生可執行檔 `hello`。

## 3. 執行程式

```bash
./hello
```

輸出：

```text
Hello, world!
```

## 4. Git 初始化與提交

```bash
git init
git add hello.c
git commit -m "Add simple C hello world example"
```

## 5. 上傳到 GitHub

先在 GitHub 建立新的 repository，然後執行：

```bash
git remote add origin <你的 GitHub repo URL>
git branch -M main
git push -u origin main
```

範例：

```bash
git remote add origin https://github.com/你的帳號/你的專案.git
```

## 6. 常見問題

- `gcc: command not found`
  - 表示你沒有安裝 C 編譯器，需安裝 GCC / MinGW / Clang。
- `fatal: remote origin already exists`
  - 先檢查現有 remote：
    ```bash
    git remote -v
    ```
  - 若需覆蓋：
    ```bash
    git remote remove origin
    ```
- `Authentication failed`
  - 需要先登入 GitHub，或使用 Personal Access Token。

## 7. 這個範例學到什麼

- `#include <stdio.h>`：包含標準輸入輸出函式庫。
- `int main() {}`：程式進入點。
- `printf(...)`：輸出文字到終端機。
- `return 0;`：表示程式正常結束。

## 8. 進一步練習建議

- 改成輸出你的名字
- 讀取使用者輸入
- 用 `for` 迴圈印出 1 到 10
- 寫簡單的加法計算器

## 9. 變更測試2
---

目前這個專案已經完成本地端提交，並準備好上傳 GitHub。
若你提供 GitHub repository URL，或我有 GitHub 權限可直接 push，我就能繼續幫你完成上傳。
