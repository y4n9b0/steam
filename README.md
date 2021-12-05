<p align="center">
   <img width="400" src="https://user-images.githubusercontent.com/8252317/83985151-9e8eaf00-a96a-11ea-9b3c-b654dc9bee2f.png">
   <p align="center">
      <img width="20" height="20" src="https://store.steampowered.com/favicon.ico"></img>
      <a href="https://github.com/1step2hell/steam-box/workflows/Update%20gist%20with%20Steam%20Playtime/badge.svg"><img src="https://github.com/1step2hell/steam-box/workflows/Update%20gist%20with%20Steam%20Playtime/badge.svg" alt="Update gist with Steam Playtime"></a>
  </p>
</p>

---
> 📌 For more pinned-gist projects like this one, check out [awesome-pinned-gists](https://github.com/matchai/awesome-pinned-gists)

## 💻 Setup

### 🎒 Prep work

> Skip step 1 and step 2 if update profile README.md only, follow [YouEclipse](https://github.com/YouEclipse/YouEclipse) .

1. Create a new public [GitHub Gist](https://gist.github.com/).
2. Create a [token](https://github.com/settings/tokens/new) with the `gist` scope and copy it.
3. Create a [Steam API key](https://steamcommunity.com/dev/apikey).
4. Find the [steam ID]((https://steamid.io))(steamID64) of your account.

### 🚀 Project setup

1. Fork this repo
2. Go to the repo **Settings > Secrets**
3. Add the following environment variables:
   - **GH_TOKEN:** The GitHub token generated above.
   - **GIST_ID:** The ID portion from your gist url: `https://gist.github.com/1step2hell/`**`f8576ab794e13a9196a2e8f1de843544`**.
   - **STEAM_API_KEY:** The steam API key you created above.
   - **STEAM_ID:** The steam ID of your account.
4. If you want to show specific games, put the ids in environmet variable **APP_ID**:
   - like `APP_ID=431960,730`
   - you can get the id of a game from the store url: `https://store.steampowered.com/app/`**730**`/CounterStrike_Global_Offensive/`

## 🕵️ How it works

- Get your games playtime from [Steamwork Web API](https://partner.steamgames.com/doc/webapi)
- Update Gist with Github API
- Use Github Actions for updating Gist  

## 📄 License

This project is licensed under [Apache-2.0](./LICENSE)
