# 🔍 Lusha Features Matrix Analysis Tool

[![GitHub Pages](https://img.shields.io/badge/deployed-GitHub%20Pages-green)](https://BenHartenBeilis.github.io/Lusha-Features-Matrix)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A powerful web-based tool for analyzing feature fragmentation across Lusha pricing versions. Built with React and designed for product managers and billing teams to understand feature evolution patterns.

## 🌟 Live Demo

**[👉 Try the Live Tool Here](https://BenHartenBeilis.github.io/Lusha-Features-Matrix)**

## 📊 Features

### 🔄 Plan Evolution Analysis
- **Track individual plans** (Professional, Enterprise, etc.) across pricing versions
- **Visual change indicators** - see when features were added (🟢) or removed (🔴)
- **Feature count trends** and change metrics between versions
- **Interactive filtering** by feature codes

### 📋 Data Requirements
Your CSV file should include these columns:
- `planName` - Plan name (e.g., "Professional", "Enterprise")
- `Pricing Version` - Numeric version (e.g., 2.6, 3.1, 4.5)
- `productCode` - Feature identifier (e.g., "oktaSso", "bulkExport")
- `productName` - Human-readable feature name

### 🎯 Key Benefits
- **Identify fragmentation** - Which features are inconsistent across versions?
- **Track evolution** - How did specific plans change over time?
- **Find patterns** - When were major feature changes made?
- **Plan consolidation** - Which versions/features can be standardized?

## 🚀 Quick Start

### Option 1: Use the Live Tool (Recommended)
1. Visit **[the live demo](https://BenHartenBeilis.github.io/Lusha-Features-Matrix)**
2. Upload your CSV file
3. Select a plan to analyze
4. Explore the feature evolution!

### Option 2: Run Locally
```bash
# Clone the repository
git clone https://github.com/BenHartenBeilis/Lusha-Features-Matrix.git
cd Lusha-Features-Matrix

# Open in your browser
open index.html
```

## 📁 Data Format Example

Your CSV should be structured like this:

```csv
planName,planCode,planDescription,Pricing Version,planActive,productCode,productName
Enterprise,enterprise,Enterprise,2.9,TRUE,oktaSso,Okta SSO
,,,,,saveToBullhorn,save to bullhorn
,,,,,bulkShowProspecting,Bulk Show Prospecting
Professional,professional,Professional,2.9,TRUE,basicSearch,Basic Search
,,,,,emailExport,Email Export
```

**Data Structure Notes:**
- First row per plan contains plan info + first feature
- Subsequent rows contain additional features for that plan
- Empty plan fields = features belong to the previous plan
- Only versions ≥ 2.6 are included in analysis

## 🖼️ Screenshots

### Plan Evolution View
![Plan Evolution Analysis](https://via.placeholder.com/800x400/4F46E5/FFFFFF?text=Plan+Evolution+View)

*Track how individual plans change across pricing versions with visual indicators for additions and removals.*

### Feature Matrix View
![Feature Matrix](https://via.placeholder.com/800x400/059669/FFFFFF?text=Feature+Matrix+View)

*See which features are available across multiple versions at a glance.*

## 🛠️ Technology Stack

- **Frontend**: React 18, Tailwind CSS
- **Data Processing**: PapaParse for CSV handling
- **Deployment**: GitHub Pages
- **No Backend**: Runs entirely in the browser for privacy

## 🔒 Privacy & Security

- **No data storage** - Files processed locally in your browser
- **No server uploads** - Everything happens client-side
- **Privacy-first** - Your billing data never leaves your device
- **Works offline** - After initial load, works without internet

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

## 📝 Use Cases

### For Product Managers
- **Feature audit** - What features exist across versions?
- **Consolidation planning** - Which versions can be merged?
- **Evolution tracking** - How did our product offerings change?

### For Billing Teams  
- **Plan complexity** - Which plans have the most fragmentation?
- **Migration planning** - What features would customers lose/gain?
- **Pricing strategy** - How do feature sets align with pricing tiers?

### For Engineering Teams
- **Technical debt** - Which features are rarely used?
- **Migration impact** - What code can be deprecated?
- **Feature lifecycle** - Track feature addition/removal patterns

## 📊 Analysis Capabilities

- **50+ pricing versions** supported (filters to ≥2.6)
- **Unlimited plans and features** - scales to your data size
- **Real-time filtering** - Search features instantly
- **Export-friendly** - Take screenshots or print reports
- **Responsive design** - Works on desktop, tablet, mobile

## 🐛 Bug Reports & Feature Requests

Found a bug or have an idea? [Open an issue](https://github.com/BenHartenBeilis/Lusha-Features-Matrix/issues) on GitHub!

## 📧 Contact

- **Created by**: [Your Name]
- **Email**: your.email@company.com
- **LinkedIn**: [Your LinkedIn Profile]

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Star This Repository

If this tool helped you analyze your feature fragmentation, please star the repository to help others discover it!

[![GitHub stars](https://img.shields.io/github/stars/BenHartenBeilis/Lusha-Features-Matrix?style=social)](https://github.com/BenHartenBeilis/Lusha-Features-Matrix/stargazers)