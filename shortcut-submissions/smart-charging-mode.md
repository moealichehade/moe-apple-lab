# Smart Charging Mode

**Created by @MoeAliChehade — Mohamad Ali Chehade**

Smart Charging Mode is an Apple Shortcut that sets an iPhone's charging limit based on the time of day or travel plans.

## Charging options

- **Night Charging:** Sets the charge limit to **80%**.
- **Morning Charging:** Sets the charge limit to **90%**.
- **Travel Mode:** Sets the limit to **100%** for a trip. Choose **Start Now** to apply it immediately, or **Schedule for Later** to save travel dates.
- **End Travel Mode:** Returns to the usual charging limit for the current time.

## Automatic charging setup

In the Shortcuts app, create a personal automation:

1. Choose the **Charger** trigger.
2. Select **Is Connected** and **Run Immediately**.
3. Add a **Text** action containing exactly `Scheduled`.
4. Add **Run Shortcut**, choose **Smart Charging Mode**, and pass the Text result as the shortcut input.

Each time the iPhone is connected to a charger, the shortcut uses these rules:

| Situation | Charge limit |
|---|---|
| During an active trip | 100% |
| 9:00 p.m. to 5:59 a.m. | 80% |
| 6:00 a.m. to 8:59 p.m. | 90% |

The charging limit is checked when the shortcut runs. If the iPhone remains plugged in across a scheduled time change, the shortcut does not automatically update the limit until it runs again.

## How it helps

Keep a lower everyday charging limit while having a simple way to switch to 100% for travel. The charger automation applies the relevant mode when you plug in.

## Availability and testing

Requires an iPhone and iOS version that expose the **Set Battery Charge Limit** Shortcuts action. Availability varies by supported iPhone model and software. The features above are the creator's supplied description; this signed build has not been independently tested in the current environment.

Created by **@MoeAliChehade**.
