---
title: Function Signatures
author: team
pubDatetime: 2025-05-21T04:06:31Z
slug: function-signature
featured: false
draft: false
tags:
  - dev
  - docs
description: Function Descriptions and signatures to help whoever's working on stuff.
---

# UI Components

## `LoginForm (ClassName?: String, ...props) : JSX.Element`

Takes in the general props as a component along with classname for Tailwind CSS configurations. Returns the Login UI. Used in `@/app/(auth-pages)/sign-in`.

## `SelectStudyType (image: string, title: string, description: string, link: string) : JSX.Element

Takes in image, title, description and a link to the page. Returns the UI for onboarding selection. Refer to [Card from NyxbUI library](https://nyxbui.design/docs/components/card) for more info. Used in `@/app/onboarding/name/study-type/page.tsx`

## `SignUpForm (ClassName?: String, ...props) : JSX.Element`

Takes in the general props as a component along with classname for Tailwind CSS configurations. Returns the sign up UI. Used in `@/app/(auth-pages)/sign-up`.

## `TailwindAdvancedEditor (returnContent) : JSX.Element`

Returns the UI for the novel text editor. For more information, read the [novel documentation](https://novel.sh/docs/introduction). Used in `@/app/notetaking`

# Schemas

## `loginFormSchema () : z.Object`

Takes in nothing. Returns the schema for the login form as shown below. DataType is a Zod Object. Refer to the [Zod React Library](https://zod.dev/) for more info.

```ts

export const loginFormSchema = z.object({
    email: z.string().email(),
    password: z.string().min(8),
})

```

## `signUpFormSchema () : z.Object`

Takes in nothing. Returns the schema for the signup form as shown below. DataType is a Zod Object. Refer to the [Zod React Library](https://zod.dev/) for more info.

```ts

export const signUpFormSchema = z.object({
email: z.string().email("Please enter a valid email address"),
password: z
    .string()
    .min(8, "Password must be at least 8 characters")
    .regex(/[A-Z]/, "Password must contain at least one uppercase letter")
    .regex(/[a-z]/, "Password must contain at least one lowercase letter")
    .regex(/[0-9]/, "Password must contain at least one number"),
confirmPassword: z.string()
}).refine((data) => data.password === data.confirmPassword, {
message: "Passwords do not match",
path: ["confirmPassword"]
})

```



# Prisma Functions



# Misc Functions



# Supabase Functions
```
