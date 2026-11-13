# Environment Setup

Complete all steps below before starting any exercise. Start by installing and logging in to Bob, then verify your extensions, find your library number, and finally connect to IBM i.

---

## 0.1 — Prerequisite Bob Setup

Check your inbox for the **"You've been invited to join your team"** email, then follow these steps to install Bob and sign in for the first time.

1. **Create your IBM ID** — Open the invitation email and click the link to create your IBM ID. This gives you an account to access IBM Bob.

2. **Download & open Bob** — Download Bob using the correct installer for your computer, then open it. If Bob asks whether to import settings from another editor, select your regular IDE or click **Skip for now**. If it asks about chat migration, click **Skip migration**.

3. **Log in to Bob** — In the Bob chat window, click **Log in to Bob**. When asked to allow Bob to sign in, click **Allow**. Bob will then ask if you want to open a link — click **Open**. This opens your browser to complete the sign-in.

4. **Verify your account is active** — Click the **gear icon** above the Bob chat window. If the chat window isn't open, click the Bob icon to the right of the center search bar to open it first.

   ![Bob settings panel showing the gear icon and General settings](img/settings-pt1.png)

   Under the **General** tab, confirm that coins are listed in your budget at **100% remaining** — this means your account is active and ready.

   > 💡 **Team dropdown:** If you have used Bob before and belong to multiple teams, a team dropdown will appear — make sure it shows a team with **Bobathon** in the name. If you only belong to one team, the dropdown may not be visible at all, which is expected.

   ![Bob team selector showing Bobathon account option](img/change-team.png)

---

## 0.2 — Verify and Install Required Extensions

Two extensions are required. The **IBM Bob Premium Package for i** is often pre-installed for your team — verify it below. The **IBM i Development Pack** must be installed manually.

1. **Open the Extensions view** — Click the Extensions icon in the Activity Bar or press `Cmd+Shift+X` (macOS) / `Ctrl+Shift+X` (Windows/Linux).

   ![Extensions icon in the Bob Activity Bar](img/open-market.png)

2. **Verify IBM Bob Premium Package for i** — Search for `"IBM Bob Premium"`. If it appears with an **Install** button, click it. If there is no Install button, skip to step 3.

   ![Searching for IBM Bob Premium in the Extensions panel](img/searching-ibm-i.png)

3. **Install IBM i Development Pack** — Search for `"IBM i Development Pack"`. This extension is **not** pre-installed — click **Install** if it does not appear under *Installed*. Reload Bob if prompted.

4. **Open Bob Settings** — Click the **Bob Settings** button in the bottom-right corner of the Bob IDE.

   ![Bob Settings button in the bottom-right corner of the Bob IDE](img/bob_settings.png)

5. **Install Premium Package for i** — Under **Add ons**, find IBM Bob Premium Package for i and click **Install**. Restart Bob if prompted.

   ![IBM Bob Premium Package for i shown next to the Add ons setting with an Install button](img/activatedd.png)

6. **Confirm it is activated** — Return to the Bob chat and click **Agent** or **+**. You should see **IBM i Developer** and **IBM i Database** modes listed.

   ![Icon in the top-right corner of Bob to return to the chat](img/sidebar-button.png)

   ![IBM i Developer and IBM i Database modes in the mode selector](img/new-modes.png)

---

## 0.3 — Choose Your Server and Library Number

Your instructor will assign you a library number. Each participant has their own copy of the FLIGHT400 application in a library named **FLGHT4nn** (e.g. FLGHT401, FLGHT402). Use only your assigned number throughout the exercises.

> ⚠️ **Action required:** Your instructor will tell you which server to use. Find the row in the table below with your assigned library number. Wherever this guide shows `4nn` or `30nn`, use the values from your row.

| Server | IP address | Private key file |
|--------|-----------|------------------|
| Primary | `169.59.252.70` | `ae_primary_key.pem` |
| Backup | `169.59.252.205` | `ae_backup_key.pem` |

Wherever this guide shows `<myIPaddress>` or `ae_<server>_key.pem`, use the values for your server. The user profile is `ITZUSER` on both.

> 💡 **Spelling note:** The library name is `FLGHT4nn` — there is **no "I"** in FLGHT.

| Student # | Library | Dev Port | React App URL |
|:---------:|---------|:--------:|---------------|
| 1  | `FLGHT401` | 3001 | `http://localhost:3001` |
| 2  | `FLGHT402` | 3002 | `http://localhost:3002` |
| 3  | `FLGHT403` | 3003 | `http://localhost:3003` |
| 4  | `FLGHT404` | 3004 | `http://localhost:3004` |
| 5  | `FLGHT405` | 3005 | `http://localhost:3005` |
| 6  | `FLGHT406` | 3006 | `http://localhost:3006` |
| 7  | `FLGHT407` | 3007 | `http://localhost:3007` |
| 8  | `FLGHT408` | 3008 | `http://localhost:3008` |
| 9  | `FLGHT409` | 3009 | `http://localhost:3009` |
| 10 | `FLGHT410` | 3010 | `http://localhost:3010` |
| 11 | `FLGHT411` | 3011 | `http://localhost:3011` |
| 12 | `FLGHT412` | 3012 | `http://localhost:3012` |
| 13 | `FLGHT413` | 3013 | `http://localhost:3013` |
| 14 | `FLGHT414` | 3014 | `http://localhost:3014` |
| 15 | `FLGHT415` | 3015 | `http://localhost:3015` |
| 16 | `FLGHT416` | 3016 | `http://localhost:3016` |
| 17 | `FLGHT417` | 3017 | `http://localhost:3017` |
| 18 | `FLGHT418` | 3018 | `http://localhost:3018` |
| 19 | `FLGHT419` | 3019 | `http://localhost:3019` |
| 20 | `FLGHT420` | 3020 | `http://localhost:3020` |
| 21 | `FLGHT421` | 3021 | `http://localhost:3021` |
| 22 | `FLGHT422` | 3022 | `http://localhost:3022` |
| 23 | `FLGHT423` | 3023 | `http://localhost:3023` |
| 24 | `FLGHT424` | 3024 | `http://localhost:3024` |
| 25 | `FLGHT425` | 3025 | `http://localhost:3025` |
| 26 | `FLGHT426` | 3026 | `http://localhost:3026` |
| 27 | `FLGHT427` | 3027 | `http://localhost:3027` |
| 28 | `FLGHT428` | 3028 | `http://localhost:3028` |
| 29 | `FLGHT429` | 3029 | `http://localhost:3029` |
| 30 | `FLGHT430` | 3030 | `http://localhost:3030` |
| 31 | `FLGHT431` | 3031 | `http://localhost:3031` |
| 32 | `FLGHT432` | 3032 | `http://localhost:3032` |
| 33 | `FLGHT433` | 3033 | `http://localhost:3033` |
| 34 | `FLGHT434` | 3034 | `http://localhost:3034` |
| 35 | `FLGHT435` | 3035 | `http://localhost:3035` |
| 36 | `FLGHT436` | 3036 | `http://localhost:3036` |
| 37 | `FLGHT437` | 3037 | `http://localhost:3037` |
| 38 | `FLGHT438` | 3038 | `http://localhost:3038` |
| 39 | `FLGHT439` | 3039 | `http://localhost:3039` |
| 40 | `FLGHT440` | 3040 | `http://localhost:3040` |
| 41 | `FLGHT441` | 3041 | `http://localhost:3041` |
| 42 | `FLGHT442` | 3042 | `http://localhost:3042` |
| 43 | `FLGHT443` | 3043 | `http://localhost:3043` |
| 44 | `FLGHT444` | 3044 | `http://localhost:3044` |
| 45 | `FLGHT445` | 3045 | `http://localhost:3045` |
| 46 | `FLGHT446` | 3046 | `http://localhost:3046` |
| 47 | `FLGHT447` | 3047 | `http://localhost:3047` |
| 48 | `FLGHT448` | 3048 | `http://localhost:3048` |
| 49 | `FLGHT449` | 3049 | `http://localhost:3049` |
| 50 | `FLGHT450` | 3050 | `http://localhost:3050` |

> 💡 The **Dev Port** is only needed for **Exercise 4**. Your React app will be reachable at the React App URL shown — provided your SSH tunnel (Exercise 4, step 4.1.1) is active.

---

## 0.4 — Connect Bob IDE to IBM i

1. **Add a new connection** — Click the IBM i icon in the Activity Bar, then click **New Connection**. Enter the host IP, the user profile `ITZUSER`, and the `ae_<server>_key.pem` private key provided in the [Box folder](https://ibm.ent.box.com/folder/437286700244?box_source=collab-auto-accept-notify-invitee&s=6l9fyh0a0icfwqeexdaqt6ramrbgqqjd). **Do not use the password here — use only the private key file.**

   ![IBM i icon in the Bob Activity Bar](img/ibmi_icon.png)

   ![IBM i connection dialog in Bob IDE](img/i-connection.png)

   > 💡 If you get a private key error, see 0.5 for instructions on setting the correct file permissions.

2. **Add your library to the User Library List** — In the Code for IBM i extension, go to **User Library List** and click **+**. Type `FLGHT4nn` and press **Enter**.

   ![User Library List section in the Code for IBM i extension](img/add-library.png)

   ![Input field prompting for library name](img/add-library-name.png)

3. **Add your library to the Object Browser** — Go to **Object Browser** and click the funnel icon or **Create new filter**. Set **Libraries** to `FLGHT4nn` and **Object types** to `*ALL`. Click **Save Settings**.

   > ⚠️ Use `*ALL`, not `*` — the wildcard `*` does not work here.

   ![Object Browser filter fields with Object types set to *ALL](img/objectfilter.jpeg)

4. **Set the workspace to Library List** — Click **+** above the Bob chat window and select **New Task in Library List**, confirming your `FLGHT4nn` library is listed.

   ![Bob scope picker showing New Task in Library List option](img/set-workspace.png)

---

## 0.5 — Set Private Key Permissions

After downloading `ae_<server>_key.pem` from the [Box folder](https://ibm.ent.box.com/folder/437286700244?box_source=collab-auto-accept-notify-invitee&s=6l9fyh0a0icfwqeexdaqt6ramrbgqqjd):

**macOS / Linux:**
```bash
chmod 600 ae_<server>_key.pem
```

**Windows (PowerShell):**
```powershell
icacls ae_<server>_key.pem /inheritance:r /grant:r "$($env:USERNAME):R"
```
