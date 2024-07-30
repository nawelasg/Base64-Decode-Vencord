


# DecodeBase64Links Plugin for Vencord

DecodeBase64Links is a Vencord plugin for Discord that allows users to decode Base64 content from any selected text within a message. This plugin simplifies the process of extracting and understanding Base64 encoded strings directly within the Discord client.

## Features

- Decode Base64 encoded strings from selected text.
- Display decoded content in a user-friendly modal.
- Copy decoded content to clipboard for easy sharing.

## Installation

### Prerequisites

Ensure you have the development version of Vencord installed. Follow the instructions below to install it.

### Installing the Development Version of Vencord

#### Prerequisites

Vencord is powered by Node.js, git, and pnpm. Make sure all of these are installed and added to your PATH.

1. **Install git**
    - [Download git](https://git-scm.com/downloads)

2. **Install Node.js**
    - [Download Node.js](https://nodejs.org/)

3. **Install pnpm**
    - [Download pnpm](https://pnpm.io/installation)

#### Verify Installations

Ensure that all installations were successful by running the following commands:

```sh
git --version
node --version
pnpm --version
```

#### Cloning the Vencord Repository

1. **Clone the Repository**
    ```sh
    git clone https://github.com/Vendicated/Vencord.git
    ```

2. **Navigate to the Vencord Directory**
    ```sh
    cd Vencord
    ```

#### Installing Dependencies

Use pnpm to install Vencord’s dependencies:

```sh
pnpm install --frozen-lockfile
```

#### Building Vencord

Compile the Vencord code:

```sh
pnpm build
```

For a development build, use:

```sh
pnpm build --dev
```

### Installing DecodeBase64Links Plugin

1. **Create Plugin Directory**

   Navigate to the Vencord source directory and create a new directory for the plugin:

   ```sh
   cd src/plugins
   mkdir DecodeBase64
   ```

2. **Add Plugin Files**

   Copy the `index.tsx` file of DecodeBase64Links into the newly created `DecodeBase64` directory.

3. **Rebuild Vencord**

   After adding the plugin files, rebuild Vencord to include the new plugin:

   ```sh
   pnpm build --dev
   ```

4. **Inject Vencord**

   Finally, inject Vencord to apply the changes:

   ```sh
   pnpm inject
   ```

### Using DecodeBase64Links

1. **Enable the Plugin**
    - Ensure the `DecodeBase64Links` plugin is enabled in your Vencord settings.

2. **Decode Base64 Content**
    - Select the Base64 encoded text in any Discord message.
    - Press on the Decode Button from the Chat Buttons.
    - A modal will appear displaying the decoded content.

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.
