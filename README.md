# Ordering systems and AI chat agents for restaurants

Portfolio and working demo. **Live demo: [sulaman0.github.io/sulamankhan](https://sulaman0.github.io/sulamankhan/)** ([English version](en.html))

I build three things for independent restaurants and small restaurant groups:

| | What it does | Why a restaurant buys it |
|---|---|---|
| **Own ordering channel** | Ordering and payment on the restaurant's own domain, with order confirmation by message and a ticket to the kitchen | Delivery platforms take up to 30% of the ticket. Uber Eats publishes 30%, and 32% on Uber One orders. A direct channel costs a flat fee instead |
| **AI chat agent** | Takes orders and table bookings in conversation, answers questions about allergens, halal, prices and opening hours, escalates to a human only when needed | Answers the calls nobody picks up during service, in several languages, around the clock |
| **Demand forecasting** | Predicts covers and orders per daypart and per location from the venue's own history, plus weather, day of week, holidays and local events | Over-prep is waste, under-prep is lost revenue. Neither shows up in the accounts as a number you can act on |

## The demo in this repo

`index.html` is a self-contained page with an interactive ordering agent built in. Click through the conversation and a full order runs end to end: the guest asks about gluten, the agent offers a gluten-free base, upsells a dip, takes payment, and sends a confirmation message. A panel alongside explains what happens at each step.

The demo restaurant, Pizzeria Nord, is fictional. This is stated on the page itself. The prices and menu are examples.

## Channel choice is per market, not assumed

The same agent runs on WhatsApp, web chat, SMS, Messenger and Instagram DM. Which one leads depends on where the guests actually are:

- **Most of Europe, Latin America, South Asia, the Middle East:** WhatsApp is where guests already are, so it usually leads.
- **The Nordics:** web chat on the venue's own site plus SMS. Denmark is the WhatsApp outlier in Europe, at roughly 22–30% against Facebook Messenger at 49%, so a WhatsApp-first build would reach a minority of guests. Internet penetration is 99% and there are 9.13 million mobile connections for 6 million people, so web plus SMS reaches everyone.
- **RCS:** worth revisiting as carriers and iOS enable it. In Denmark that is expected in 2027.

The product does not change. The channel does.

## Running it

No build step, no dependencies, no server, no API keys. One HTML file with inline CSS and JavaScript.

```
git clone https://github.com/sulaman0/sulamankhan.git
cd sulamankhan
open index.html          # or: python3 -m http.server 8000
```

## Repository contents

```
index.html    Danish version, live at /
en/index.html English version, live at /en/
README.md     this file
```

Both pages carry a `DA | EN` switcher in the top right. The links between them are relative, so renaming the repository will not break them.

## Working with me

I start every engagement with a free demo built on the restaurant's own menu and branding, usually within 48 hours of the first conversation. There is no commitment attached to it. If it is useful we talk about price, and if it is not, nothing has been spent.

**Sulaman Khan** · Freelance developer
se.sulaman.khan@gmail.com · +92 316 785 2626 (also on WhatsApp)
