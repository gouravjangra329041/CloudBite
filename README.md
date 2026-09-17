# CloudBite
I have made an app called "Cloud Bite". This is a food delivery app and I built this during my Internship.
The idea was simple: one app, two sides.

Customers can browse the menu (with veg/non-veg tags, spice levels and prep times), build a cart with a proper bill breakdown (GST, delivery fee, free delivery above ₹500), place an order, and then track it live through every stage — Placed → Accepted → Preparing → Ready → Out for delivery → Delivered.

The kitchen owner gets a separate PIN-protected dashboard to manage the order queue, move orders through each status, and mark dishes sold out — which instantly reflects on the customer side.

One design decision I'm glad we made: order status changes are business operations, so they belong only to the owner. The customer's only action is placing the order — everything after that is in the kitchen's control. Modeling the whole order as a state machine kept both views perfectly in sync.

Built with React Native + Expo, with AsyncStorage for persistence — so the entire demo runs with zero backend cost.
