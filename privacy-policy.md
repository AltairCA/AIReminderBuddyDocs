# Privacy Policy for AIReminderBuddy

**Effective date:** June 26, 2026  
**Last updated:** June 26, 2026

This Privacy Policy describes how **AIReminderBuddy** (“the App,” “we,” “us,” or “our”) handles information when you use our mobile application on Android and iOS.

**Developer / data controller:**  
Michika Perera  
Contact: altairserver@gmail.com

If you have questions about this policy, contact us at the email above.

---

## Summary

AIReminderBuddy is a **local-first** reminder app. Your reminders, lists, photos, and settings are stored **on your device**. We do **not** operate a user account system and we do **not** collect your personal data on our own servers in the current version of the App.

Optional AI features use **your own API key** and send content **directly from your device** to the AI provider you choose (Google Gemini, OpenRouter, or OpenAI). We do not receive or store that content on our servers.

---

## 1. Information the App Stores on Your Device

The App stores the following data locally on your phone or tablet:

| Data type | Purpose | Stored where |
|-----------|---------|--------------|
| Reminders and schedules | Notify you when tasks are due | SQLite database on device |
| Reminder history (done/skipped) | Show your activity | SQLite database on device |
| Scanned objects and library entries | Organize items you track | SQLite database on device |
| Photos you capture or import | Display in your library; optional AI analysis | App-private storage on device |
| Text descriptions you enter | Manual reminders and AI text suggestions | SQLite database on device |
| Lists and list items | Shopping, todo, and other lists | SQLite database on device |
| App settings | Notifications, default times, onboarding state | SQLite database on device |
| AI provider choice and connection status | Remember which AI service you connected | SQLite database on device (no secret keys) |
| API keys (if you connect AI) | Authenticate with your chosen AI provider | Device secure storage (Expo SecureStore) |

We do **not** sync this data to our servers in the current version of the App.

---

## 2. Information Sent to Third-Party AI Providers (Optional)

AI features are **optional**. If you choose to connect an AI provider and use scan or text-suggestion features, the App sends requests **directly from your device** to that provider’s API using **your API key**.

Depending on what you do, the following may be sent to your chosen provider:

- **Photos** you select or capture (compressed/resized as JPEG before sending)
- **Text** you type (object descriptions, list content, shared text)
- **System prompts** required to request structured task suggestions

Supported providers (you choose one):

| Provider | Privacy policy |
|----------|----------------|
| Google (Gemini API) | https://policies.google.com/privacy |
| OpenRouter | https://openrouter.ai/privacy |
| OpenAI | https://openai.com/policies/privacy-policy |

**Important:**

- We do **not** receive, store, or review the content you send to AI providers.
- Your relationship with the AI provider (billing, quotas, retention, and how they use API inputs) is governed by **that provider’s terms and privacy policy**.
- You can disconnect AI at any time in Settings, which removes your stored API key from the device.
- You can use the App **without AI** by creating reminders and lists manually.

When using OpenRouter, the App may include identifying headers required by that service (such as app name and referer URL). No user account information is included.

---

## 3. Device Permissions

The App may request the following permissions:

| Permission | Why we ask |
|------------|------------|
| **Camera** | Take photos to scan objects or add list items |
| **Photos / media library** | Import images you already have |
| **Notifications** | Deliver local reminders when tasks are due |

Permissions are used only for these features. You can deny permissions, though some features will not work without them.

The App does **not** use the microphone and does not request microphone access on Android or iOS.

---

## 4. Share Into the App

If you share text or an image from another app into AIReminderBuddy, that content is handled **on your device** to create reminders or lists. Shared content is only sent to an AI provider if you explicitly use an AI-powered action and have connected a provider.

---

## 5. What We Do **Not** Collect

In the current version of the App, we do **not**:

- Require you to create an account
- Operate our own backend that stores your reminders or photos
- Sell your personal information
- Show third-party advertising
- Use analytics or advertising SDKs to track you across apps
- Collect precise location data
- Access your contacts, calendar, or SMS

---

## 6. Local Notifications

Reminders are scheduled using your device’s local notification system. Notification content (titles, times) stays on your device and is delivered by your operating system. We do not send push notifications through our own servers.

---

## 7. Children’s Privacy

AIReminderBuddy is not directed at children under 13 (or the minimum age required in your country). We do not knowingly collect personal information from children. If you believe a child has provided information through the App, contact us and we will help you understand how to remove locally stored data (typically by uninstalling the App or clearing app data).

---

## 8. Data Retention and Deletion

Data remains on your device until you:

- Delete individual reminders, objects, lists, or images inside the App
- Disconnect an AI provider (removes the API key from secure storage)
- Clear the App’s storage in your device settings
- Uninstall the App

Uninstalling the App removes locally stored data from your device, subject to your operating system’s behavior.

We do not retain copies of your data on our servers in the current version.

---

## 9. Security

We use reasonable measures available on mobile platforms, including:

- Storing API keys in the device’s secure storage
- Keeping app data in the app’s private sandbox
- Sending AI requests over HTTPS

No method of storage or transmission is 100% secure. You are responsible for keeping your device and API keys safe.

---

## 10. International Users

If you use optional AI features, your content may be processed in countries where your chosen AI provider operates (for example, the United States). Those providers’ privacy policies apply to that processing.

---

## 11. Your Rights

Depending on where you live, you may have rights to access, correct, delete, or restrict processing of your personal information.

Because the App stores data **locally** and we do not operate a cloud account system, you can exercise most rights directly by managing or deleting data in the App or uninstalling it.

To contact us about privacy requests, email: **altairserver@gmail.com**

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. We will post the updated policy at the same URL and change the “Last updated” date. Continued use of the App after changes means you accept the updated policy.

---

## 13. Google Play Data Safety (Summary)

For Google Play’s Data safety form, the current App generally aligns with:

| Category | Declaration guidance |
|----------|---------------------|
| Data collected by **you (developer)** | None, or minimal technical data only if you add analytics later |
| Data shared with **third parties** | Only when user opts into AI — photos/text sent to user’s chosen AI provider |
| Data encrypted in transit | Yes (HTTPS for AI API calls) |
| Data deletion | User can delete in-app or uninstall |
| Account required | No |

*Update this table if you add analytics, crash reporting, accounts, or a backend.*

---

## 14. Contact

**Michika Perera**  
Email: **altairserver@gmail.com**  
App package ID: `com.aireminderbuddy.app`
