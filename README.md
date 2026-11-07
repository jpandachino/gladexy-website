# Gladexy website

Ordering website for Gladexy (Lagos). Orders go to WhatsApp and are also saved in Firebase.

## WhatsApp numbers
In `index.html`, search for `WHATSAPP_NUMBER`:
- `WHATSAPP_NUMBER` = main line (2348034545059). Every order goes here first.
- `BACKUP_NUMBER` = second line (2348115774461). Offered to customers if the main line doesn't reply.

## Firebase (database + Google Analytics)
Project: gladexy-45bb7. The settings are in the `firebaseConfig` block near the end of `index.html`.
- Customers (name, phone) are saved to the `customers` collection.
- Orders and event requests are saved to the `orders` collection when the customer taps "Send on WhatsApp".
- View them in Firebase: Databases & Storage > Firestore > Data.
- Visitor stats: Firebase > Analytics, or analytics.google.com.
