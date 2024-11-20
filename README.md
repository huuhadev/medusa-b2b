<h1 align="center"> Medusa B2B Commerce Starter </h1>

<p align="center">Customizable B2B ecommerce monorepo built with <a href="https://medusajs.com/" target="_blank">Medusa 2.0</a> & Next.js Storefront</p>
<br>

## Table

- [Prerequisites](#prerequisites)
- [Overview](#overview)
  - [Features](#features)
  - [Demo](#demo)
- [Quickstart](#quickstart)

&nbsp;

## Prerequisites

⚠️ We use turborepo to manage this monorepo and have tested this only with the below versions:

- ✅ yarn version 3.5
- ✅ node 20
- ✅ Postgres 15
- ✅ Medusa 2.0

&nbsp;

## Overview

#### Features

- **Company Management**. Customers can manage their company and invite employees.
- **Spending Limits**. Company admins can assign spending limits to its employees
- **Bulk add-to-cart**. Customers can add multiple variants of a product to their cart at once.
- **Quote Management**. Customers & Merchants can communicate, accept or reject quotes
- **Order Edit**. Merchants can edit orders or quotes - add/remove item, update quantity & price management and more.
- **Full ecommerce support**
  - Product Pages
  - Product Collections & Categories
  - Cart & Checkout
  - User Accounts
  - Order Details
- **Full Next.js 14 support**
  - App Router
  - Next fetching/caching
  - Server components/actions
  - Streaming
  - Static Pre-Rendering

&nbsp;

#### Demo

#### Quote Management

<img align="right" src="https://github.com/user-attachments/assets/110c99e8-18ba-49e5-8955-84a058b597c7" alt="image" style=: />
&nbsp;

#### Company Management

<img align="right" src="https://github.com/user-attachments/assets/361702ce-d491-4509-a930-4361ab3b4126" alt="image" style=: />
&nbsp;

#### Product Page

<img align="right" src="https://github.com/user-attachments/assets/2cd8a3ff-5999-49af-890a-4bac7b6f2f15" alt="image" style=: />
&nbsp;

#### Cart Summary

<img align="right" src="https://github.com/user-attachments/assets/095f5565-992e-4c74-acdc-a44bd905e59b" alt="image" style=: />
&nbsp;

&nbsp;

## Quickstart

#### Setup storefront & API
⚠️ Create a Postgres database named `medusa_b2b` and make sure the Postgres server is running locally.

Clone the repository
```bash
git clone https://github.com/huuhadev/medusa-b2b.git
```

Go to the folder
```bash
cd ./medusa-b2b
```

Install dependencies & setup medusa storefront & backend
```bash
yarn install && yarn setup
```

Start Servers - storefront & backend

```bash
yarn dev
```

#### Setup publishable key[.env](../storefront/.env)

- ✅ Visit Admin: [Publishable Key](http://localhost:9000/app/settings/publishable-api-keys)
  - <b>Credentials</b>:
    - <b>email</b>: `huuhadev@gmail.com`
    - <b>password</b>: `password`
- ✅ Copy token key of "Webshop"
- ✅ Open file - `apps/storefront/.env`
- ✅ Add token to this var - `NEXT_PUBLIC_MEDUSA_PUBLISHABLE_KEY`

Visit the following links to see the Medusa storefront & admin

- [Medusa Admin](http://localhost:9000/app)
- [Medusa Storefront](http://localhost:8000)
