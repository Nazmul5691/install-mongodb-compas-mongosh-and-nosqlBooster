# MongoDB Setup with GUI Tools and Shell Access

This guide helps you install and work with MongoDB using graphical interfaces (MongoDB Compass, NoSQLBooster) and the command line (mongosh).


---

## 📦 Installing MongoDB Community Server (with Compass & mongosh)

1. **Download MongoDB Community Edition:**
   - Open your browser and search: `MongoDB Community Server download`
   - Go to the official MongoDB website.
   - Select your OS: **Windows x64**
   - Download the installer.

2. **Install MongoDB:**
   - Run the installer.
   - Choose: **Complete Setup**
   - Click **Next** → **Next** → **Install** to finish the setup.

3. **Launch MongoDB Compass (GUI):**
   - Open **MongoDB Compass** from the start menu.
   - Click **Connect** to connect to the default local MongoDB instance.

4. **Use mongosh (MongoDB Shell) from Compass:**
   - Open the **mongosh** tab in Compass.
   - Run basic commands:

     ```bash
     show dbs                                  # View all databases
     use practice                              # Create/use a database named 'practice'
     db.createCollection("test")               # Create a collection
     db.getCollection("test").insertOne({ name: "trying to learn mongodb" })  # Insert document
     db.getCollection("test").find()           # Query documents
     ```

---

## 💻 Setting up mongosh in Command Prompt (CMD)

1. **Install mongosh separately:**
   - Search `MongoDB Shell download` in Google.
   - Download the `.msi` package and install it.

2. **Add mongosh to system PATH:**
   - Go to: `C:\Program Files\MongoDB\Server\<version>\bin`
   - Copy the full path (replace `<version>` with your installed version, e.g., `8.0`).
   - Open **System Properties** → **Environment Variables**
   - Add the copied path to the **Path** variable.

3. **Use mongosh in CMD:**
   - Open Command Prompt and type:

     ```bash
     mongosh
     show dbs
     use practice
     db.getCollection("test").find()
     ```

---

## 🖥️ Using Other MongoDB GUIs

You can also use third-party tools like **NoSQLBooster** or **Studio 3T**.

### ✅ Using NoSQLBooster

1. **Download NoSQLBooster:**
   - Search: `NoSQLBooster download`
   - Choose **Windows** version and download.

2. **Install and Run:**
   - Install the software.
   - Open NoSQLBooster.

3. **Connect to MongoDB:**
   - Click **Connect** → **New Connection**
   - Set name to `localhost` → Click **Save & Connect**

4. **Create Collection & Run Commands:**
   - Create a new collection (e.g., `test`).
   - Use the editor to run commands.
   - Press `Ctrl + Enter` to execute commands.

---

## ✅ You're Ready!

You now have multiple ways to interact with MongoDB:
- MongoDB Compass (GUI)
- mongosh via Compass or CMD
- NoSQLBooster (GUI)

Happy coding with MongoDB!
