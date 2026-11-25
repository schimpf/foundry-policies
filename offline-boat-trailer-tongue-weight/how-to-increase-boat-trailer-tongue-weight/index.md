# How to Increase Boat Trailer Tongue Weight

> Four ways to fix low boat trailer tongue weight, with formulas and a worked example. The same math works in reverse for a heavy tongue.

- Web: https://apps.schimpf.es/offline-boat-trailer-tongue-weight/how-to-increase-boat-trailer-tongue-weight/
- App: Boat Trailer Tongue Weight, https://apps.schimpf.es/offline-boat-trailer-tongue-weight/index.md
Your boat trailer should carry about 7 to 10 percent of its weight on the hitch. If yours carries less, the trailer can sway. If it carries more, the tow vehicle squats and steering gets light. This page shows four ways to change tongue weight and the math to size each one.

The formulas are the ones in the [boat trailer tongue weight calculator](/boat-trailer-tongue-weight-calculator) page. Positions are in inches from the axle, positive toward the coupler.

## Start with the numbers

You need three values:

- **W**: total trailer weight (lb)
- **L**: coupler-to-axle distance (in)
- **M**: total moment about the axle (lb-in). Tongue weight = M / L.

Aim for the middle of the range, 8.5 percent. The moment you need is 0.085 x W x L. The moment you are missing is:

**Need = 0.085 x W x L - M**

A positive Need means the tongue is too light. A negative Need means it is too heavy.

Example: W = 3,794 lb, L = 168 in, M = 40,000 lb-in.

- Tongue weight = 40,000 / 168 = 238 lb, which is 6.3 percent. Too light.
- Target moment = 0.085 x 3,794 x 168 = 54,178 lb-in.
- Need = 14,178 lb-in.

## 1. Drain water first

A livewell, baitwell or ballast tank behind the axle pulls the tongue up. Water weighs 8.34 lb per gallon. Draining it removes weight that was lifting the tongue. This costs nothing and takes a minute, so try it first. See [boat fuel and water weight per gallon](/boat-fuel-and-water-weight-per-gallon).

The new percent is (M - water moment) / L / (W - water weight). Do not drain a tank ahead of the axle. That makes the tongue lighter.

## 2. Move the boat forward

Sliding the boat toward the bow stop moves its weight, and everything fixed to it, ahead. Every pound moves the same distance, so:

**Shift = Need / boat and load weight**

In the example, the items on the trailer weigh 3,794 - 1,200 = 2,594 lb. Shift = 14,178 / 2,594 = 5.47 inches. Round to 5.5 inches forward.

- New moment = 40,000 + 5.5 x 2,594 = 54,267 lb-in
- New tongue weight % = 54,267 / 168 / 3,794 = 8.5 percent

Use a negative shift to move the boat back when the tongue is too heavy. Do not push the bow past the winch post stop. The app assumes the bow rests at the winch post, about 18 inches behind the coupler.

## 3. Move gear

Heavy gear can move too: batteries not wired in, coolers, anchors, tools, a spare tire. Move one item by:

**Distance = Need / item weight**

A 150 lb pile of gear needs 14,178 / 150 = 94.5 inches. That is a long way, so gear alone rarely fixes a big gap. It is a good fine adjustment. Keep gear reasonably placed: moving it too far behind the axle loses the benefit and loads the frame badly. The app limits gear to at most 60 percent of the coupler-to-axle distance behind the axle.

## 4. Move the axle

Moving the axle rearward moves every load forward relative to it and lengthens the lever L. With a shift of d inches rearward:

**New percent = (M + W x d) / (L + d) / W**

The shift needed is:

**d = Need / (W - 0.085 x W)**

In the example: d = 14,178 / (3,794 - 322.5) = 14,178 / 3,471.5 = 4.08 inches. Round to 4 inches rearward.

- New moment = 40,000 + 3,794 x 4 = 55,176 lb-in
- New L = 172 in
- New percent = 55,176 / 172 / 3,794 = 8.5 percent

Use a negative d (axle forward) when the tongue is too heavy.

Moving an axle is real work on a welded or bolted frame. It changes the trailer as the maker built it, so check with the trailer maker or a trailer shop. Many trailers have an adjustable axle position, and some have a sliding bunk or winch stand for the boat.

## If the tongue is too heavy

Reverse every move:

- Move the boat back on the bunks.
- Move gear toward the stern.
- Move the axle forward.
- Move heavy items out from behind the axle, such as a full livewell, to ahead of it.

## Check after the change

1. Recalculate. A fix for the tongue can push the rear axle or another rating over its limit.
2. Compare tongue weight with the maximum on your hitch and receiver labels.
3. Check the axle load, trailer GVWR, tow rating and GCWR.
4. Weigh the rig if you can. An estimate can be off by a lot.

## Do it in the app

The Boat Trailer Tongue Weight app for Android lists these moves for you. When your loaded tongue weight is outside 7 to 10 percent, it suggests draining a livewell, moving the boat, moving a piece of gear, or moving the axle, with the distance and the resulting percent. It works offline at the ramp.

Treat all results as estimates. You are responsible for a safe and legal tow.
