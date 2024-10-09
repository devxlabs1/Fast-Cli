<div align="center" style="background-color: #f8f9fa; border-radius: 8px; padding: 20px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);"> 
    <h1 style="text-align:center; color: #007bff;">✨ Fast</h1>
    <p style="font-size: 20px; padding: 0; color: #555;">Latest Version: 1.0.8</p>
    <p style="font-size: 16px; color: #333;">⚡ <strong style="color: #333;">Fast</strong> is your go-to solution for developing MIT App Inventor 2 extensions efficiently. Wave goodbye to @Annotations and hello to a efficient development experience!</p>
</div>


---

### 🚀 Key Features

- **Java 8 Support:** Harness the power of lambda expressions (e.g., `()->`) for cleaner, more concise code.
- **Kotlin Compatibility:** Enjoy the flexibility of working with non-component classes, enhancing your coding prowess.
- **Multi-Component Support:** Manage and integrate multiple components within your extensions effortlessly for added functionality.
- **Red Helper Blocks:** Utilize new red helper blocks to assist you better during the development process.
- **ProGuard Integration:** Benefit from the latest version of ProGuard for optimal code protection and optimization.
- **Size Optimizer:** Efficiently reduce AIX size, even without ProGuard, ensuring your projects remain lightweight.
- **Manifest Attributes:** Easily declare manifest attributes directly in `AndroidManifest.xml` for improved configuration.
- **Intelligent Code Suggestions:** Receive real-time code suggestions in VSCode, Eclipse, IntelliJ IDEA, and Android Studio, making coding smoother than ever.
- **Class Filtering:** Keep your workspace tidy by filtering out unnecessary MIT App Inventor provided classes.
- **Auto Project Migration:** Transition your projects to the Fast framework seamlessly with minimal hassle.
- **Jetifier Support:** Migrate Android support libraries to AndroidX effortlessly, ensuring your projects are always up-to-date.

---

### 🖥️ Supported Operating Systems

- **Windows**
- **Linux**
- **macOS**
- **Android (Termux/UserLand)**

---

### ⚙️ Installation

#### For Windows

1. **Open PowerShell.**
2. Run the following command:

   ```powershell
   iwr https://raw.githubusercontent.com/jewelshkjony/fast-cli/main/scripts/install/install.ps1 -useb | iex

#### For Linux

1. **Open your terminal.**
2. Execute the command below:

   ```bash
   curl https://raw.githubusercontent.com/jewelshkjony/fast-cli/main/scripts/install/install.sh -fsSL | sh
   ```

---

### 🛠️ Available Commands

Below are the commands you can use:

| Command   | Description                                              |
| --------- | -------------------------------------------------------- |
| `build`   | Build the project in the current working directory.      |
| `create`  | Create a new extension project in the current directory. |
| `clean`   | Clean project build caches in the current directory.     |
| `sync`    | Sync project dependencies in the current directory.      |
| `jetify`  | Migrate Android support libraries to AndroidX.           |
| `migrate` | Migrate the Rush/extension-template project to Fast.     |
| `propfix` | Automatically add the category attribute where required. |

---

### 📝 Arguments

You can use the following arguments with your commands:

| Argument   | Description                                                  |
| ---------- | ------------------------------------------------------------ |
| `-r`       | Execute the ProGuard task (use with the `build` command).    |
| `-o`       | Optimize the extension size even without ProGuard (use with `build`). |
| `-x`       | Generate the DEX Bytecode using the deprecated dexer (use with `build`). |
| `rush`     | Indicate it's a Rush project for the `migrate` command.      |
| `template` | Indicate it's an extension-template project for the `migrate` command. |
| `ai2`      | Indicate it's an App Inventor sources project for the `migrate` command. |
| `rush2`    | Indicate it's a Rush2 project for the `migrate` command (Upcoming). |

---

### 🌟 Quick Start 

1. **Install Fast:** Follow the [installation instructions](#installation) above to get started.
   
2. **Get Started:** Create your new extension project with:

   ```bash
   fast create <extension-name>
   ```

   **Example:**
   ```bash
   fast create example
   ```

   Next, fill in the required parameters:
   - **Package Name:** `com.yourcompany`
   - **Author Name:** `your Name`
   
3. **Edit Your Project:** After the project is created, navigate to `your-project/src/your-name/extension-name/extension.java` and edit it according to your needs.

4. **Build Your Extension:** Run the following command to build your extension:

   ```bash
   fast build
   ```

**Important Note:** If you're using Java 8, it won't compile by default. You will need to enable `desugar_sources` by setting it to `true` in `your-extension-directory/fast.yml` (it’s set to `false` by default).

5. **Add Dependencies:** If you're using any dependencies, make sure to include them in your `fast.yml`.

6. **Compile Again:** After making these changes, compile your project again.

