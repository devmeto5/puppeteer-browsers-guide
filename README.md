# Step-by-Step Guide for Installing and Launching Browsers with `@puppeteer/browsers`

## Step 1: Install Node.js and npm

Before you begin, make sure you have **Node.js** and **npm** (Node.js package manager) installed. If they are not installed, download and install them from the [official Node.js website](https://nodejs.org/).

Check that they are installed using the following commands:

```bash
node -v
npm -v
```

You should see the versions of Node.js and npm.

## Step 2: Using `@puppeteer/browsers` to Manage Browsers

The `@puppeteer/browsers` package is used to manage browsers via CLI. It allows you to download, install, and launch browsers and drivers.

### 2.1. Viewing Help for Commands

To get familiar with the available commands, use `npx` to run the help command:

```bash
npx @puppeteer/browsers --help
```

- **Help for all commands**:
  
  ```bash
  npx @puppeteer/browsers --help
  ```

- **Help for installing browsers**:

  ```bash
  npx @puppeteer/browsers install --help
  ```

- **Help for launching browsers**:

  ```bash
  npx @puppeteer/browsers launch --help
  ```

### 2.2. Installing Browsers and Drivers

1. **Download the latest Chrome version for testing (Stable Channel)**:

   ```bash
   npx @puppeteer/browsers install chrome@stable
   ```

2. **Download a specific Chrome version**:

   ```bash
   npx @puppeteer/browsers install chrome@116.0.5793.0
   ```

3. **Download the latest Chrome version for a specific major release**:

   ```bash
   npx @puppeteer/browsers install chrome@117
   ```

4. **Download the latest ChromeDriver version for the Canary channel**:

   ```bash
   npx @puppeteer/browsers install chromedriver@canary
   ```

5. **Download a specific ChromeDriver version**:

   ```bash
   npx @puppeteer/browsers install chromedriver@116.0.5793.0
   ```

6. **Download other drivers (e.g., Firefox or Edge)**:

   You can also download drivers for other browsers, such as Firefox or Edge, using similar commands. For example, to install Firefox:

   ```bash
   npx @puppeteer/browsers install firefox@latest
   ```

### 2.3. Launching a Browser

After installing a browser, you can launch it using the following command:

```bash
npx @puppeteer/browsers launch chrome
```

You can also specify a specific version to launch, for example:

```bash
npx @puppeteer/browsers launch chrome@116.0.5793.0
```

## Conclusion

Using `@puppeteer/browsers` simplifies the installation and management of browsers for automation and testing purposes. In this guide, we covered how to install and launch browsers using the CLI, providing an easy way to manage browser versions for your testing needs.

