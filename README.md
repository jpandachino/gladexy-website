# Gladexy website

Ordering website for Gladexy (Lagos). Orders are sent to WhatsApp, so no accounts or database are needed.

## Going live checklist
In `index.html`, search for `WHATSAPP_NUMBER`:
- Testing: `2348115774461`
- Live: change to `2348034545059`

Also change `const TESTING = true;` to `false`.

## Firebase (database + Google Analytics)
Project: gladexy-45bb7. The settings are in the `firebaseConfig` block near the end of `index.html`.
- Customers (name, phone) are saved to the `customers` collection.
- Orders and event requests are saved to the `orders` collection when the customer taps "Send on WhatsApp".
- View them in Firebase: Databases & Storage > Firestore > Data.
- Visitor stats: Firebase > Analytics, or analytics.google.com.
