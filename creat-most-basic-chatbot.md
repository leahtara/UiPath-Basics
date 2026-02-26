 ***creating a New Process***.

---

# 🚀 Step-by-Step: Create a New Process in UiPath

## ✅ Step 1: Open UiPath Studio

When you open UiPath Studio, you’ll see the **Start screen**.

If you don’t:

* Click **Home** (top left corner)

---

## ✅ Step 2: Click “New Project”

On the left side, you will see:

* Process
* Library
* Test Automation
* Blank Solution

👉 Click **Process**

(That’s what we want for a chatbot.)

---

## ✅ Step 3: Configure Your Project

A new window will open.

Fill in:

* **Name:** `SimpleChatbot`
* **Location:** Leave default
* **Description:** (Optional) “My first chatbot”
* **Compatibility:** Choose **Windows**

Then click:

👉 **Create**

---

## ✅ Step 4: You’re Inside the Project 🎉

Now you’ll see:

* A file called **Main.xaml**
* A big blank workflow area
* The **Activities** panel on the left

That’s it. You have created your first UiPath process.

---

Now we’ll build the **most basic chatbot possible** so you understand UiPath first. Then we can upgrade it to AI.


---

# 🎯 Goal

User types something → Bot responds.

---

# ✅ STEP 1 — Add a Sequence

In the middle (Designer panel):

1. Click inside `Main.xaml`
2. In the Activities panel (left side), search:

   ```
   Sequence
   ```
3. Drag **Sequence** into the workflow area

You should now see a **Sequence block**.

---

# ✅ STEP 2 — Add Input Dialog (User types message)

1. In Activities search:

   ```
   Input Dialog
   ```
2. Drag it inside the Sequence

Now configure it (right side Properties panel):

* **Title** → `"Chatbot"`
* **Label** → `"Ask me something"`
* **Result** → Click `+` → Create Variable → Name it:

```
userInput
```

Type should be:

```
String
```

Done ✅

---

# ✅ STEP 3 — Add Message Box (Bot reply)

Now:

1. Search:

   ```
   Message Box
   ```
2. Drag it below the Input Dialog

In the **Text** field, type:

```
"Hello! You said: " + userInput
```

---

# ▶️ STEP 4 — Run It

Click **Run** (top ribbon ▶️)

You’ll see:

* A popup asking you something
* Then it replies with what you typed

🎉 BOOM. That’s your first chatbot.

---
