<div align="center">

<img src="https://raw.githubusercontent.com/Studio1HQ/Studio1HQ/main/assets/banners/velt-email-composer.webp" alt="MailCraft Email Composer with Velt: A Tiptap email composer with inline comments, presence and notifications" width="100%" />

<br />
<br />

# MailCraft Email Composer with Velt

### A Tiptap email composer with inline comments, presence and notifications

MailCraft is a Next.js email composer built on Tiptap. Velt adds inline comments on selected text, a comments sidebar, presence and notifications.

<br />

[![Built by Studio1](https://img.shields.io/badge/Built_by_Studio1-f97316?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNjAgMTYwIiBmaWxsPSJub25lIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTAgMzVDMCAxNi42ODA3IDE0LjA3NDQgMS42NDg0NCAzMiAwLjEyNjk1M1YxNDFINTEuMDUyM0M1Mi40MzA4IDEzNy4zNDQgNTQuNzQ0NiAxMzMuNjg5IDU3Ljk5MzggMTMwLjAzM0M2MS4xNDQ2IDEyNi41MDggNjQuNjg5MiAxMjMuNDQgNjguNjI3NyAxMjAuODI5QzcyLjU2NjIgMTE4LjM0OSA3Ni4zNTY5IDExNi43ODIgODAgMTE2LjEyOVY4Ni43NTQ0Qzc1LjQ3MDggODcuOTI5MiA3MS4zODQ2IDg5LjY5MTkgNjcuNzQxNSA5Mi4wNDE1QzY0IDk0LjUyMjUgNjAuNzUwOCA5Ny40NiA1Ny45OTM4IDEwMC44NTRDNTYuNTM0NSAxMDIuNzIgNTUuMjU0NSAxMDQuNjU5IDU0LjE1MzkgMTA2LjY3MVYwSDEyNUMxNDQuMzMgMCAxNjAgMTUuNjY5OSAxNjAgMzVWMTI1QzE2MCAxNDQuMzMgMTQ0LjMzIDE2MCAxMjUgMTYwSDEyNFYxOEgxMDQuOTQ4QzEwMy41NjkgMjEuNjgxNiAxMDEuMjU1IDI1LjM2MjggOTguMDA2MiAyOS4wNDQ0Qzk0Ljg1NTQgMzIuNTk0MiA5MS4zMTA4IDM1LjY4NDEgODcuMzcyMyAzOC4zMTRDODMuNDMzOCA0MC44MTIgNzkuNjQzMSA0Mi4zODk2IDc2IDQzLjA0NzRWNzIuNjMwNEM4MC41MjkyIDcxLjQ0NzMgODQuNjE1NCA2OS42NzI0IDg4LjI1ODUgNjcuMzA1N0M5MiA2NC44MDc2IDk1LjI0OTIgNjEuODQ5MSA5OC4wMDYyIDU4LjQzMDdDOTkuNDY1NSA1Ni41NTEzIDEwMC43NDUgNTQuNTk4NiAxMDEuODQ2IDUyLjU3MjNWMTYwSDM1QzE1LjY3IDE2MCAwIDE0NC4zMyAwIDEyNVYzNVoiIGZpbGw9IiNmZmZmZmYiLz48L3N2Zz4K)](https://studio1hq.com)
[![Built with Velt](https://img.shields.io/badge/Built_with_Velt-141414?style=for-the-badge)](https://velt.dev)

[Velt docs](https://docs.velt.dev) &nbsp;·&nbsp; [Velt](https://velt.dev) &nbsp;·&nbsp; [More examples](https://github.com/Studio1HQ) &nbsp;·&nbsp; [studio1hq.com](https://studio1hq.com)

</div>

<br />

## Overview

MailCraft is an email composer built with Next.js, Tiptap, shadcn/ui and [Velt](https://velt.dev). Users write an email in a rich text editor and discuss it by commenting on selected text.

Velt provides inline comments through `@veltdev/tiptap-velt-comments`, along with presence, notifications and a comments sidebar. Two predefined users (Nany and Mary) let you test collaboration in one browser.

## Features

- **Rich text editor**: Tiptap with a bubble menu on selection, headings, lists, bold and italic.
- **Inline comments**: Select text and add a comment with the Velt Tiptap integration.
- **Presence**: `VeltPresence` shows who is viewing the email.
- **Notifications**: `VeltNotificationsTool` shows a bell for new comments and replies.
- **Comments sidebar**: `VeltCommentsSidebar` and `VeltSidebarButton` manage all discussions.
- **User switching**: Switch between Nany and Mary.
- **Dark and light mode**: Both themes supported, with a responsive layout.

## Tech stack

| Layer | Tool |
| --- | --- |
| Framework | [Next.js](https://nextjs.org) (App Router), [React](https://react.dev), TypeScript |
| Editor | [Tiptap](https://tiptap.dev) |
| Collaboration | [Velt](https://velt.dev) (`@veltdev/react`, `@veltdev/tiptap-velt-comments`) |
| UI | [Tailwind CSS](https://tailwindcss.com), [shadcn/ui](https://ui.shadcn.com), [Lucide](https://lucide.dev) |
| State | [Zustand](https://zustand-demo.pmnd.rs) |

## Getting started

### Prerequisites

- Node.js 18 or later
- npm or yarn
- A Velt API key from the [Velt console](https://console.velt.dev)

### Installation

```bash
git clone https://github.com/Studio1HQ/velt-email-composer.git
cd velt-email-composer
npm install
```

### Environment variables

Create a `.env` file in the project root.

| Variable | Description |
| --- | --- |
| `NEXT_PUBLIC_VELT_ID` | Your Velt API key. |

```bash
echo "NEXT_PUBLIC_VELT_ID=your_velt_api_key_here" > .env
```

### Run

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## How it works

```text
app/(app)/layout.tsx       Velt and theme providers
app/(app)/page.tsx         email composer page
components/EmailEditor.tsx Tiptap editor with Velt integration
components/EditorFooter.tsx footer with formatting options
components/email-composer.tsx main composer layout
components/navbar.tsx      navigation with Velt tools
constant/general.ts        initial editor content
helper/userdb.ts           user management and state
hooks/use-theme.tsx        theme hook
```

The editor uses the Velt Tiptap integration:

```tsx
import { TiptapVeltComments, renderComments, addComment } from "@veltdev/tiptap-velt-comments";

TiptapVeltComments.configure({ persistVeltMarks: false });  // editor extension
renderComments({ editor, editorId, commentAnnotations });   // render existing comments
addComment({ editor, editorId });                           // add a comment on the selection
```

## Resources

- [Velt documentation](https://docs.velt.dev): SDK guides.
- [Velt](https://velt.dev): product site.
- [Tiptap guide](https://tiptap.dev/docs): editor docs.
- [shadcn/ui](https://ui.shadcn.com): UI components.

<br />

---

<div align="center">

<a href="https://studio1hq.com">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Studio1HQ/website/main/brand/studio1-logo-on-dark.svg" />
    <img src="https://raw.githubusercontent.com/Studio1HQ/website/main/brand/studio1-logo-on-light.svg" alt="Studio1" width="160" />
  </picture>
</a>

Built by **[Studio1](https://studio1hq.com)**, the technical content and DevRel partner for devtool teams. Made with [Velt](https://velt.dev).<br />
Browse more open-source examples at [github.com/Studio1HQ](https://github.com/Studio1HQ).

[![Website](https://img.shields.io/badge/studio1hq.com-0b0807?style=for-the-badge&logo=googlechrome&logoColor=white)](https://studio1hq.com)
[![Book a call](https://img.shields.io/badge/Book_a_strategy_call-f97316?style=for-the-badge&logo=googlecalendar&logoColor=white)](https://cal.com/studio1/collab)
[![X](https://img.shields.io/badge/%40Studio1HQ-141414?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Studio1HQ)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/studio1hq/)

<sub><a href="https://studio1hq.com">studio1hq.com</a> · Technical content, docs, video and DevRel for devtools</sub>

</div>
