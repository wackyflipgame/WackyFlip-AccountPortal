# 🧑‍🚀 WackyFlip-AccountPortal

**The Official Player Account Dashboard for Wacky Flip**

This repository contains the **frontend interface** for managing [Wacky Flip](https://wackyflip.com) player accounts. From editing your avatar and linking devices to customizing privacy and game preferences — this is where **players take control** of their Wacky Flip identity.

Accessible from **[wackyflip.com/account](https://wackyflip.com/account)** (or via mobile in-app browser), the **WackyFlip-AccountPortal** provides a clean, responsive interface for every kind of flipper.

---

## 🎯 Features

| Feature               | Description                                                             |
| --------------------- | ----------------------------------------------------------------------- |
| 📝 Profile Editor     | Customize display name, avatar, bio, and player tags                    |
| 📱 Device Linking     | Manage cross-device access and platform connections (Web, iOS, Android) |
| ⚙ Preferences         | Set gameplay, UI, notification, and control settings                    |
| 🔐 Privacy & Security | Control data sharing, visibility, and session management                |
| 🌐 Linked Accounts    | Connect social logins (Google, Apple, Discord, etc.)                    |
| 🎮 Game Stats Preview | See your total flips, best scores, and rank highlights                  |

---

## 🛠 Tech Stack

* **Frontend**: React + TypeScript
* **State Management**: Zustand
* **Styling**: Tailwind CSS + ShadCN UI
* **API Integration**: via `WackyFlip-API`
* **Auth**: Integrated with `WackyFlip-Auth`
* **Analytics**: Events routed to `WackyFlip-Stats`

---

## 📁 Folder Structure

```
WackyFlip-AccountPortal/
├── components/
│   ├── ProfileCard.tsx
│   ├── DeviceList.tsx
│   └── SettingsTabs/
├── pages/
│   ├── index.tsx
│   ├── preferences.tsx
│   └── security.tsx
├── hooks/
├── utils/
├── public/
├── styles/
└── README.md
```

---

## 🧪 Example

```tsx
// components/ProfileCard.tsx
export function ProfileCard({ player }) {
  return (
    <Card>
      <Avatar src={player.avatarUrl} />
      <h2>{player.displayName}</h2>
      <p>Rank: {player.rank}</p>
      <Button>Edit Profile</Button>
    </Card>
  );
}
```

---

## 🔐 Security & Compliance

* OAuth 2.0 / OpenID Connect
* CSRF + XSS Protection
* GDPR-ready data management
* Integration with `WackyFlip-Push` for account alerts

---

## 🔄 Future Plans

* [ ] Avatar Marketplace (custom skins, hats, etc.)
* [ ] 2FA integration with email/SMS apps
* [ ] Parental controls for young players
* [ ] Player-to-player profile viewing

---

## 🧑‍💻 Contributing

We welcome contributions from the community or internal Wacky Flip teams!
To begin:

```bash
git clone https://github.com/wackyflip/WackyFlip-AccountPortal.git
pnpm install
pnpm dev
```

---

## 📜 License

MIT © 2025 [Wacky Flip Studios](https://wackyflip.com)
