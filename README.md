# Laravel React Feature

An application for managing features with roles, permissions, voting and comments using Laravel, React, Inertia and Server-Side Rendering (SSR).

## Features

1. User registration and login
2. Roles and permissions (Admin, Commenter, User)
3. Admin can manage features, manage their own comments, edit users’ roles and vote
4. Commenter can vote and manage their own comments
5. User can vote on features
6. Features CRUD with pagination
7. Upvote and downvote system for features
8. Comment system for discussion on features

## Local Setup

> [!TIP]
> Make sure your environment is set up properly. You will need PHP 8.2, Composer and Node.js installed and the commands `php`, `composer`, `node` and `npm` should be available in your terminal.

1. Clone the project
2. Go to the project's root directory from terminal
3. Copy `.env.example` into `.env` file `cp .env.example .env`
4. Open and adjust your `.env` parameters
5. Run `composer install`
6. Set application key `php artisan key:generate --ansi`
7. Execute migrations and seed data: `php artisan migrate --seed`
8. Run `npm install`
9. Run `composer run dev` for local development

## Setup SSR

Follow the steps above including step 8, after which

1. Open terminal and execute `npm run build` to build react assets
2. Then start artisan server `php artisan serve`
3. Open another terminal and execute `php artisan inertia:start-ssr` to start server side rendering server

## Test Users

Use these accounts after running the project locally:

**Admin User**

```
Email: admin@example.com
Password: password
```

**Commenter User**

```
Email: commenter@example.com
Password: password
```

**Regular User**

```
Email: user@example.com
Password: password
```
