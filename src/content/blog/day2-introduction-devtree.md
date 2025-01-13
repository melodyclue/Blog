---
author: literal
pubDatetime: 2025-01-13T13:00:00+09:00
modDatetime: 2025-01-13T13:00:00+09:00
title: Day2 - 個人開発者向けリンクツリー 「DevTree」
slug: day2-introduction-devtree
featured: true
draft: false
tags:
  - 個人開発
description: 個人開発者向けリンクツリー 「DevTree」を作っていきます！
---

## 課題と解決策

Day1のPSBLフレームワークをもとに、「DevTree」という個人開発者向けのリンクツリーを作ってみる

まずは課題と解決策をぱぱっと考えてみた

### 課題

- プロダクトへの導線は作れるものの、詳細な説明や更新履歴などを加えにくい。
- GitHubやnoteなど、関連情報への導線を複数追加しにくい。

### 解決策

プロダクトへの導線だけではなく、その概要や、ステータス（開発中、ベータ版など）、GitHubやnote、Xへの複数リンクなどの更新履歴や関連情報も加えたい。一番シンプルなやり方としては、リンクをクリックしたときにサイドバーやモーダルを表示して、プロダクトの詳細を見せるというのが良いかも

## Build

課題と解決策を考えたら、まず技術スタックを定義する。
自分の場合こんな感じ

| トピック       | スタック                      |
| -------------- | ----------------------------- |
| データベース   | Supabase Postgresql           |
| 認証           | ArcticのGitHub Authentication |
| 画像           | Cloudflare R2                 |
| フレームワーク | React Router v7               |
| Third Party    | Tailwindcss / shadcn/ui       |

### とりあえず作ること

- プロダクトのCRUD
- 認証・プロフィール設定

一旦こんな感じで作ってみる！！
