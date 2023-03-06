# 我的餐廳論壇
[deployed Heroku](https://pure-retreat-00432.herokuapp.com/)

利用node.js打造餐廳論壇，提供餐廳列表，使用者能進一步查看特色內容、地址及預約電話，也可以使用收藏功能或是追蹤使用者心目中的美食達人，用美食填滿使用者的每一天！

## 功能
1. 查看所有餐廳列表
2. 查看餐廳資料
3. 前後台系統
4. 管理員增刪改查餐廳
5. 篩選功能
6. 使用者註冊登入登出
7. 使用者收藏餐廳
8. 使用者追蹤使用者
9. 餐廳評論功能

## 使用介面
![alt 使用介面圖示](https://github.com/thk61159/forum-express-grading/blob/main/forum.png?raw=true "我的餐廳論壇使用介面")

## 如何使用
1. 開啟終端機(terminal)，輸入如下將專案複製到電腦中
```shell
 git clone https://github.com/thk61159/forum-express-grading.git
```
2. 進入此專案資料夾，安裝各種套件
```shell
 cd restaurantList
 npm install
```
3. 在MySQL建立專案資料庫並修改/config/config.json資料庫連線之帳號密碼
4. 圖片上傳功能，如果需要用到imgurAPI需要去註冊使用，或是使用 /helpers/file-helpers.localFileHandler
5. 建立.env檔並輸入
需要設定的參數請參照.env.example檔
6. 新增種子資料(可省略)
```shell
npm run seed
```
3. 運行我的餐廳論壇
```shell
 npm run start
```
4. 拜訪我的餐廳論壇網頁
```shell
 http://localhost:3000/
```

##開發工具
* Visual Studio Code 
* Node.js v14.16.0
* Bootstarp
* MySQL


# README (from AC)

1. Fork
2. git clone

## 初始化
### Initialize
```
git remote add upstream https://github.com/ALPHACamp/forum-express-grading.git  # 建立上游連線
npm install
```

### 設定資料庫
需要與 config/config.json 一致

```
create database forum;
```

### 執行測試
```
npm run test
```

## 下載作業規格
以 R01 為例

```
git checkout -b R01           # 開新分支
git merge origin/R01-test     # 下載作業規格
npm run test                  # 直到綠燈全亮

git add .
git commit -m "...."
```

## 繳交作業

```
git push origin R01           # 上傳本地進度
```

接著改成到 GitHub 來發 PR。

## 共用帳號
請一律設定下面 2 組帳號以利驗收：
* 第一組帳號有 admin 權限：
  * email: root@example.com
  * password: 12345678
* 第二組帳號沒有 admin 權限：
  * email: user1@example.com
  * password: 12345678