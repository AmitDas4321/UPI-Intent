<p align="center">
  <img src="./public/assets/banner.png" alt="UPI Intent Banner" width="900">
</p>

<h1 align="center">
  💳 UPI Intent
</h1>

<p align="center">
  <strong>A developer-focused UPI Intent & Deep-Link reference for exploring app-specific payment intents across popular Indian UPI applications.</strong>
</p>

<p align="center">
  <a href="https://github.com/AmitDas4321/UPI-Intent">
    <img src="https://img.shields.io/github/stars/AmitDas4321/UPI-Intent?style=for-the-badge" alt="GitHub Stars">
  </a>
  <a href="https://github.com/AmitDas4321/UPI-Intent/network/members">
    <img src="https://img.shields.io/github/forks/AmitDas4321/UPI-Intent?style=for-the-badge" alt="GitHub Forks">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-1.0.0-22C55E?style=flat-square" alt="Version 1.0.0">
  <img src="https://img.shields.io/badge/UPI-Intent-16A34A?style=flat-square" alt="UPI Intent">
  <img src="https://img.shields.io/badge/Deep%20Links-Mobile%20Apps-2563EB?style=flat-square" alt="Deep Links">
  <img src="https://img.shields.io/badge/Android-Compatible-3DDC84?style=flat-square&logo=android&logoColor=white" alt="Android">
  <img src="https://img.shields.io/badge/Developer-Reference-7C3AED?style=flat-square" alt="Developer Reference">
</p>

---

# 💳 About UPI Intent

**UPI Intent** is an independent developer reference project for exploring **UPI payment deep links, app-specific URI schemes, and payment intent formats** used by popular Indian UPI applications.

The project provides a centralized reference for developers who want to understand how UPI payment intents are structured and how application-specific payment flows can be invoked from supported environments.

### Included UPI Applications

- 📱 **PhonePe**
- 💙 **Paytm**
- 🟣 **MobiKwik**
- 🔴 **Airtel Payments**
- 🇮🇳 **Standard UPI**

The repository focuses on practical intent examples, URI formats, parameters, encoding, testing, and integration concepts.

> ⚠️ **Important:** App-specific intent schemes may be undocumented, private, version-dependent, restricted, or changed without notice. This repository is intended for developer reference, testing, research, and educational purposes.

---

# ✨ Key Features

### 🔗 UPI Deep-Link Reference

Explore different URI schemes used to initiate UPI-related payment flows.

### 📱 App-Specific Intents

Reference intent formats for:

- PhonePe
- Paytm
- MobiKwik
- Airtel Payments

### 🇮🇳 Standard UPI URI

Reference the commonly used:

```text
upi://pay
```

payment URI.

### 🔐 Encoded Payload Examples

Understand intents containing:

- Base64-encoded JSON
- Base64-encoded UPI URI
- URL query parameters

### 🧪 Testing Examples

Includes examples suitable for mobile, Android, browser, and ADB-based testing.

### 📚 Developer Documentation

Clear parameter references and implementation examples for developers.

---

# 🔗 Exact UPI Intent Examples

The following intent strings are preserved **exactly as provided**.

No parameters, values, encoding, casing, or URI structure has been modified.

---

## 📱 PhonePe

```text
phonepe://native?data=eyJwMnBQYXltZW50Q2hlY2tvdXRQYXJhbXMiOnsiY2hlY2tvdXRUeXBlIjoiQ09MTEVDVCIsImluaXRpYWxBbW91bnQiOjEwMCwibm90ZSI6eyJ0eXBlIjoidGV4dCIsIm1lc3NhZ2UiOiJUWE4yMDI2MTAwNTE0Mzc1OERFNjdEMjE2In0sInN1cHBvcnRlZEluc3RydW1lbnRzIjotMX0sImNvbnRhY3QiOnsidHlwZSI6IkVYVEVSTkFMX01FUkNIQU5UIiwibmFtZSI6IkJsdWVPcmJpdCBEZXZzIiwidnBhIjoicGF5dG1xcjVtZWV2b0BwdHlzIn19&id=p2ppayment
```

### Scheme

```text
phonepe://native
```

### Flow Identifier

```text
id=p2ppayment
```

The provided intent contains a Base64-encoded `data` payload.

---

## 💙 Paytm

```text
paytmmp://cash_wallet?pa=paytmqr5meevo@ptys&pn=null&cu=INR&tn=AT2eashwkl4n&am=1&featuretype=money_transfer
```

### Scheme

```text
paytmmp://cash_wallet
```

### Parameters

| Parameter | Value |
| :--- | :--- |
| `pa` | `paytmqr5meevo@ptys` |
| `pn` | `null` |
| `cu` | `INR` |
| `tn` | `AT2eashwkl4n` |
| `am` | `1` |
| `featuretype` | `money_transfer` |

---

## 🟣 MobiKwik

```text
mobikwik://upi/verifyVpa?vpa=paytmqr5meevo@ptys&amount=1&note=TXN20261005143758DE67D216
```

### Scheme

```text
mobikwik://upi/verifyVpa
```

### Parameters

| Parameter | Value |
| :--- | :--- |
| `vpa` | `paytmqr5meevo@ptys` |
| `amount` | `1` |
| `note` | `TXN20261005143758DE67D216` |

---

## 🔴 Airtel Payments

```text
myairtel://app/airtelpay?screenName=scan_pay&source=scan_device_native&journey=pay&qrString=dXBpOi8vcGF5P3BhPXBheXRtcXI1bWVldm9AcHR5cyZwbj1udWxsJmN1PUlOUiZ0bj1BVDJlYXNod2tsNG0mYW09MQ==
```

### Scheme

```text
myairtel://app/airtelpay
```

### Parameters

| Parameter | Value |
| :--- | :--- |
| `screenName` | `scan_pay` |
| `source` | `scan_device_native` |
| `journey` | `pay` |
| `qrString` | Base64-encoded UPI URI |

---

# 📚 Intent Reference

| Application | Intent Scheme | Type |
| :--- | :--- | :--- |
| 📱 PhonePe | `phonepe://native` | App-specific |
| 💙 Paytm | `paytmmp://cash_wallet` | App-specific |
| 🟣 MobiKwik | `mobikwik://upi/verifyVpa` | App-specific |
| 🔴 Airtel Payments | `myairtel://app/airtelpay` | App-specific |
| 🇮🇳 Standard UPI | `upi://pay` | Standard |

---

# 🇮🇳 Standard UPI Intent

The standard UPI payment URI generally uses:

```text
upi://pay
```

A common structure is:

```text
upi://pay?pa=<UPI_ID>&pn=<PAYEE_NAME>&am=<AMOUNT>&cu=INR&tn=<NOTE>
```

Example:

```text
upi://pay?pa=merchant@upi&pn=Demo%20Merchant&am=100&cu=INR&tn=TXN123
```

---

# 🧩 Standard UPI Parameters

| Parameter | Description | Example |
| :--- | :--- | :--- |
| `pa` | Payee UPI ID | `merchant@upi` |
| `pn` | Payee name | `Demo Merchant` |
| `am` | Payment amount | `100` |
| `cu` | Currency | `INR` |
| `tn` | Transaction note | `TXN123` |
| `tr` | Transaction/reference ID | `REF123` |
| `mc` | Merchant category code | `0000` |
| `url` | Reference URL | `https://example.com` |

---

# ⚙️ Generate Standard UPI Intent

A standard UPI intent can be generated dynamically:

```javascript
const upiId = "merchant@upi";
const merchantName = "Demo Merchant";
const amount = "100";
const transactionId = "TXN123456";

const upiIntent =
  `upi://pay` +
  `?pa=${encodeURIComponent(upiId)}` +
  `&pn=${encodeURIComponent(merchantName)}` +
  `&am=${encodeURIComponent(amount)}` +
  `&cu=INR` +
  `&tn=${encodeURIComponent(transactionId)}`;

console.log(upiIntent);
```

Result:

```text
upi://pay?pa=merchant@upi&pn=Demo%20Merchant&am=100&cu=INR&tn=TXN123456
```

---

# 🌐 Web Integration

A web application can attempt to launch a UPI intent using:

```javascript
function openUPIPayment() {
  const upiUrl =
    "upi://pay" +
    "?pa=merchant@upi" +
    "&pn=Demo%20Merchant" +
    "&am=100" +
    "&cu=INR" +
    "&tn=TXN123";

  window.location.href = upiUrl;
}
```

Example:

```html
<button onclick="openUPIPayment()">
  Pay with UPI
</button>
```

On compatible mobile devices, the operating system may open an installed UPI application capable of handling the URI.

> Browser behavior depends on the device, browser, installed applications, and operating-system restrictions.

---

# 📱 Android Integration

A standard UPI intent can be launched through Android's `ACTION_VIEW`:

```java
Uri uri = Uri.parse(
    "upi://pay" +
    "?pa=merchant@upi" +
    "&pn=Demo%20Merchant" +
    "&am=100" +
    "&cu=INR" +
    "&tn=TXN123"
);

Intent intent = new Intent(Intent.ACTION_VIEW, uri);

startActivity(intent);
```

Android will attempt to resolve the URI using compatible applications installed on the device.

---

# 🔐 Base64 Payloads

Some application-specific intents use Base64-encoded data.

For example, a JSON payload can be encoded using:

```javascript
const payload = {
  amount: 100,
  vpa: "merchant@upi",
  note: "TXN123"
};

const encoded = btoa(JSON.stringify(payload));

console.log(encoded);
```

The payload can be decoded using:

```javascript
const decoded = JSON.parse(atob(encoded));

console.log(decoded);
```

### ⚠️ Security Notice

Base64 is **encoding, not encryption**.

Do not use Base64 to protect:

- API keys
- Passwords
- Access tokens
- Private credentials
- Encryption keys
- Sensitive payment information

---

# 🧪 Testing UPI Intent

For Android development, a standard UPI URI can be tested using ADB:

```bash
adb shell am start -a android.intent.action.VIEW \
-d "upi://pay?pa=merchant@upi&pn=Demo%20Merchant&am=1&cu=INR&tn=TEST123"
```

App-specific URI schemes can also be tested on devices where the corresponding application is installed and supports the scheme.

### Testing Checklist

- [ ] Compatible Android device
- [ ] UPI application installed
- [ ] Valid UPI ID
- [ ] Correct amount
- [ ] Correct URL encoding
- [ ] Unique transaction/reference ID
- [ ] Intent opens successfully
- [ ] Payment flow completes successfully
- [ ] Payment independently verified

---

# 🔐 Payment Security

Opening a UPI intent does **not** mean that a payment has been completed.

The following are different states:

```text
Intent Created
      ↓
Intent Opened
      ↓
Payment Screen Displayed
      ↓
User Approves Payment
      ↓
Bank / PSP Processing
      ↓
Payment Result
      ↓
Server-side Verification
```

Therefore:

```text
Intent Opened ≠ Payment Successful
```

A production payment system should independently verify the transaction before marking an order as paid.

---

# 💡 Recommended Payment Flow

```text
Create Order
     ↓
Generate Transaction ID
     ↓
Generate UPI Intent
     ↓
Open UPI Application
     ↓
Customer Completes Payment
     ↓
Payment Processing
     ↓
Verify Payment
     ↓
Reconcile Transaction
     ↓
Mark Order as PAID
```

The backend should remain the source of truth for payment status.

---

# 🛡️ Security Recommendations

For production implementations:

- Generate transaction IDs server-side.
- Never trust payment status supplied by the client.
- Verify the expected amount on the backend.
- Verify the destination UPI ID.
- URL-encode dynamic parameters.
- Prevent transaction/reference ID reuse.
- Maintain payment logs.
- Implement transaction reconciliation.
- Handle cancelled payments.
- Handle failed payments.
- Handle pending transactions.
- Keep API credentials on the server.
- Never expose private credentials inside intent URLs.
- Do not treat an opened intent as proof of payment.

---

# 📦 Use Cases

UPI intents can be useful for:

- 🛒 E-commerce checkout
- 📱 Mobile applications
- 🌐 Web-based payment pages
- 💳 Payment collection systems
- 🧾 Invoice payment links
- 🏪 Merchant applications
- 🤖 Automated payment workflows
- 📊 Internal payment testing
- 🧪 UPI interoperability research

---

# 🚀 Roadmap

- [x] Standard UPI Intent
- [x] PhonePe Intent reference
- [x] Paytm Intent reference
- [x] MobiKwik Intent reference
- [x] Airtel Payments Intent reference
- [x] Intent parameter documentation
- [x] Exact intent examples
- [x] Base64 payload examples
- [x] JavaScript examples
- [x] Android examples
- [x] Web examples
- [x] ADB testing examples
- [ ] UPI Intent Generator
- [ ] UPI QR Generator
- [ ] Web-based Intent Builder
- [ ] Intent Validation Utility
- [ ] UPI App Compatibility Matrix
- [ ] Additional UPI Application References
- [ ] Community-maintained Intent Database

---

# 🤝 Contributing

Contributions are welcome.

If you discover a new UPI intent format, parameter, compatibility behavior, or application-specific URI, you can contribute it to the project.

### Contribution Guidelines

1. Fork the repository.
2. Create a new branch.
3. Add or update the relevant documentation.
4. Include a reproducible example.
5. Mention the application version and device where possible.
6. Test the intent before submitting.
7. Submit a Pull Request.

Example:

```bash
git clone https://github.com/AmitDas4321/UPI-Intent.git

cd UPI-Intent

git checkout -b add-new-intent

git add .

git commit -m "docs: add new UPI intent reference"

git push origin add-new-intent
```

---

# ⚠️ Disclaimer

This repository is an **independent developer reference project**.

It is **not affiliated with, endorsed by, or officially supported by**:

- PhonePe
- Paytm
- MobiKwik
- Airtel Payments
- NPCI
- Any bank
- Any UPI application
- Any payment provider

Application-specific URI schemes may be:

- Undocumented
- Private
- Version-dependent
- Restricted
- Changed without notice
- Removed in future application updates

The exact intent examples in this repository are provided for **reference, research, development, testing, and educational purposes**.

For production payment integrations, developers should use the official documentation, APIs, SDKs, and supported integration methods provided by the respective payment provider.

---

# 👨‍💻 Author

<p align="center">
  <a href="https://github.com/AmitDas4321">
    <img src="https://github.com/AmitDas4321.png" width="120" style="border-radius: 50%;" alt="Amit Das">
  </a>
</p>

<p align="center">
  <b>Amit Das</b><br>
  Full Stack Developer
</p>

<p align="center">
  <a href="https://github.com/AmitDas4321">
    <img src="https://img.shields.io/badge/GitHub-AmitDas4321-181717?style=for-the-badge&logo=github" alt="GitHub">
  </a>
  <a href="https://amitdas.site">
    <img src="https://img.shields.io/badge/Portfolio-amitdas.site-0A66C2?style=for-the-badge" alt="Portfolio">
  </a>
</p>

---

# 📜 License

This project is licensed under the **MIT License**.

---

<p align="center">
  <b>Built for developers exploring UPI Intent 🚀</b><br>
  Made with ❤️ by <a href="https://amitdas.site">Amit Das</a>
</p>