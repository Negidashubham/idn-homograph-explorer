# IDN Homograph Explorer

An interactive educational cybersecurity project for learning how **IDN homograph attacks**, **Unicode homoglyphs**, and **Punycode** can make different domain names appear visually similar.

🌐 **Live Website:** https://idnhomograph.org

---

## About the Project

IDN Homograph Explorer demonstrates how characters from different Unicode writing systems can resemble ordinary Latin characters.

For example, two characters may look almost identical to a person while having completely different Unicode code points.

The project is designed to make this concept easier to understand through interactive visualisations rather than only technical explanations.

---

## Interactive Learning Modes

### Character Explorer

Explore individual Latin characters and their visually similar Unicode alternatives.

The visual graph shows the relationship between the original character and possible lookalikes, including information such as:

- Unicode code point
- Script family
- Languages
- Visual similarity
- Character risk profile

### Attack Examples

Explore prepared examples of lookalike domains using different Unicode scripts.

Examples demonstrate:

- Cyrillic substitutions
- Greek lookalikes
- Latin extensions
- Unicode character differences
- Punycode representation
- Visual similarity between domains

### Try It Yourself

Enter a domain and interactively explore possible Unicode lookalike substitutions.

The lab provides:

- Character-by-character substitutions
- Unicode script filtering
- Visual domain comparison
- Punycode output
- Variant selection
- Risk information

---

## What is an IDN Homograph Attack?

Internationalized Domain Names (IDNs) allow Unicode characters to be used in domain names.

Some Unicode characters from different writing systems are visually similar.

For example:

| Character | Script | Unicode |
|---|---|---|
| `a` | Latin | `U+0061` |
| `а` | Cyrillic | `U+0430` |

Although these characters can appear almost identical, computers treat them as different characters.

This visual similarity can potentially be abused to create deceptive domain names.

---

## What is Punycode?

DNS fundamentally operates using ASCII-compatible domain names.

Unicode domain labels can therefore be represented using **Punycode**, which commonly begins with:

`xn--`

The explorer helps demonstrate the relationship between:

**Displayed Unicode domain → Unicode characters → Punycode representation**

---

## Educational Purpose

This project was created for:

- Cybersecurity education
- Security awareness training
- Unicode security demonstrations
- IDN and Punycode learning
- Phishing awareness
- Defensive domain analysis

The goal is to help users understand why visually inspecting a domain name alone may not always be sufficient.

---

## Privacy

The interactive demonstrations are designed to run directly inside the user's browser.

Domain transformations do not require a user account or database.

---

## Technology

The project is intentionally lightweight and built primarily with:

- HTML5
- CSS3
- JavaScript
- Unicode / IDN concepts
- Client-side Punycode processing

The website is hosted using **Cloudflare Pages** with source control and deployment through **GitHub**.

---

## Project Structure

```text
idn-homograph-explorer/
│
├── index.html
├── IDN_Homograph_Fraud_Demo.html
├── robots.txt
├── sitemap.xml
└── README.md
