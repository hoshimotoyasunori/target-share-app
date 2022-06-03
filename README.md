# SNS - Clone App

## 機能

```bash
email & password アクセス
プロフィール編集機能
投稿機能
いいね機能
メモ機能
```

## database

User

```bash
id
email
password
```

Profile

```bash
id
nickname
userProfile
img
created_at
```

Post

```bash
id
title
userPost
img
liked
created_at
```

Memo

```bash
id
memo
userMemo
```

## API Endpoint

```bash
api/register/      [POST]  新規アカウント作成
api/myprofile/     [GET]  ログインユーザーのProfile取得
api/memo/       [GET/POST/PUT]  メモの取得と投稿
api/post/          [GET/POST/PUT/PATCH]  投稿の取得、作成、更新、一部更新
api/profile/       [GET/POST/PUT]  Profileの取得、作成、更新
authen/jwt/create/ [POST]  JWTトークン取得
```

## Backend

DjangoRestFramework & JWT 認証

```bash
python3 -m venv venv
source venv/bin/activate
```

```bash
pip install django==3.0.7
pip install djangorestframework==3.10
pip install djangorestframework-simplejwt==4.6.0
pip install PyJWT==2.0.0
pip install djoser
pip install django-cors-headers
```

Django プロジェクト作成

```bash
django-admin startproject api_target .
django-admin startapp api
```

起動確認

```bash
python manage.py runserver
```

## Frontend

```bash
React Hooks & Redux Toolkit
Typescript & Material UI
Formik + Yup
```

redux-toolkit & typescript プロジェクト作成

```bash
npx create-react-app . --template redux-typescript --use-npm
```

起動確認

```bash
npm start
```

追加でinstall

```bash
npm i @material-ui/core --legacy-peer-deps
npm i @material-ui/icons --legacy-peer-deps
npm i @material-ui/lab --legacy-peer-deps
npm i react-modal --legacy-peer-deps
npm i --save-dev @types/react-modal
npm install formik
npm install -S yup
npm install axios --save
npm install react-icons --save
```
