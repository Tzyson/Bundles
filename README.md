## ⚠️ **IMPORTANT INFO BEFORE YOU START** ⚠️  
- You can get all Fortnite's Battle Royale cosmetics from **[Fortnite.GG](https://fortnite.gg/cosmetics)**.

### 🔑 **Requirements for Cosmetics and the Bundle to Work**
1. **Cosmetics must be from Chapter 3 Season 1 (Version 19.10) or earlier, Anything newer won’t work.**
2. **Bundle prices should be either 2800, 3800 or 5000 based on how wanted/good the bundle is.**  
3. **Follow the correct Cosmetic ID format.**  *Incorrect formatting will break the shop.**

---

### 🛠️ **PART 1: Understanding the File Structure**  
- The bundle uses a **JSON file** to define which items appear and their prices. Here's what the basic structure looks like:

```json
{
    "BUNDLE NAME": "EXAMPLE LOCKER",
    "idType": "AthenaCharacter:CID_LOL",
    "id1Type": "AthenaPickaxe:Pickaxe_LOL",
    "id2Type": "AthenaGlider:Glider_Lol",
    "id3Type": "AthenaDance:EID_LOL",
    "id4Type": "AthenaBackpack:Backpack_LOL",
    "bundleid": "",
    "price": 5000,
    "introduction": {
        "chapter": "AXYS",
        "season": "19"
    },
    "shopHistory": null
}
```
### 🔍 **Breaking Down the Code:**
- **`idType`, `idType1`, etc.:** Slots for the cosmetics by their **Cosmetic ID**.  
- **`bundleid`, etc.:** This is the bundleid it self, you can either put in your username on Axys or simply leave it empty.  
- **`price`:** How many V-Bucks the bundle will cost.  
---

### 🏷️ **PART 2: Correct Cosmetic ID Formatting**  
- Each item has a unique ID called a **Cosmetic ID**. The format depends on the item type.

### ✅ **General Format:**  
```
ItemType:CosmeticID
```

### 🔖 **Examples by Item Type:**  
- **Skins:** `AthenaCharacter:Character_AxysLol`  
- **Emotes (Dances):** `AthenaDance:Dance_Flare`  
- **Pickaxes:** `AthenaPickaxe:Pickaxe_AxysLol`  
- **Gliders:** `AthenaGlider:Glider_StarSurfer`  
- **Wraps:** `AthenaItemWrap:Wrap_Galaxy`  
- **Loading Screens:** `AthenaLoadingScreen:LoadingScreen_Galactic`  
- **Skydiving Contrails:** `AthenaSkyDiveContrail:Contrail_Rainbow`  

**💡 NOTE:** Always wrap your **Cosmetic ID** in double quotes (`""`), or the config will break.

---

### 🏪 **PART 3: Filling Out Your Item Shop**  
- Here’s how to set up each item in your shop:  

- **`itemGrants`:** Add the formatted Cosmetic ID for the item you want to sell.  
- **`price`:** Set the cost using Fortnite’s official V-Bucks prices.  

### ✅ **Example Config Setup:**  
```json
{
    "BUNDLE NAME": "TZY LOCKER",
    "idType": "AthenaCharacter:CID_A_202_Athena_Commando_F_Division",
    "id1Type": "AthenaPickaxe:Pickaxe_ID_363_LollipopTricksterFemale",
    "id2Type": "AthenaGlider:Glider_ID_176_BlackMondayCape_4P79K",
    "id3Type": "AthenaDance:EID_TwistDaytona",
    "id4Type": "AthenaBackpack:BID_229_LuckyRiderMale",
    "bundleid": "",
    "price": 3800,
    "introduction": {
        "chapter": "AXYS",
        "season": "19"
    },
    "shopHistory": null
}
```

---

## 🚫 **PART 4: Common Mistakes to Avoid**  

🔴 **DON’T:**  
- ❌ Forget double quotes around your **Cosmetic ID**. Example: `AthenaCharacter:Character_AxysLol` → `"AthenaCharacter:Character_AxysLol"`  
- ❌ Add commas to numbers. Use `1200`, not `1,200`.  
- ❌ Use cosmetics from versions after **Chapter 3 Season 1** (*they won’t work.*)

✅ **DO:**  
- ✔️ Double-check every **Cosmetic ID** format.  
- ✔️ Use **Visual Studio Code** to spot errors automatically.  

---

## 💡 **PART 5: Pro Tips for a Smoother Setup**  

1. 🖥️ **Install Visual Studio Code (VS Code):**  
   - It highlights errors in your JSON automatically.  
   - Helps keep formatting clean and consistent.  

2. 🤖 **Use AI tools (like ChatGPT) to validate your JSON:**  
   - Quickly check if your formatting is correct before testing in-game.  


How can your Bundle be picked? Open an issue on this repository and every day i will be picking 1 bundle every day.
Create a issue on this github repo with your bundle.json for me to pick your bundle.
