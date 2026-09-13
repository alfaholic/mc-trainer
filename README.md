# MC Trainer

One-file motorcycle skills trainer for the iPhone Home Screen. Parking lot, mini cones, 20 minutes a session.

MSF-inspired: drills follow the skill families taught in the Motorcycle Safety Foundation Basic RiderCourse (friction zone, weave, quick stop, swerve, U-turn box). Not affiliated with MSF; no MSF range cards or course material are reproduced here.

## Put it on your phone (once, ~5 minutes, no terminal)

1. On github.com, click **+ → New repository**. Name it `mc-trainer`, keep it **Public**, click **Create repository**.
2. On the new repo page, click **uploading an existing file**. Drag in these four files: `index.html`, `sw.js`, `manifest.json`, `icon.png`. Click **Commit changes**.
3. Repo **Settings → Pages**. Under *Build and deployment*, Source = **Deploy from a branch**, Branch = **main**, folder **/ (root)**. Save.
4. Wait a minute, refresh that page. It shows your URL: `https://<your-username>.github.io/mc-trainer/`.
5. On the iPhone, open that URL in **Safari** (must be Safari). Tap the **Share** button → **Add to Home Screen** → Add.
6. Open it from the Home Screen once while online. From then on it works with no signal.

## Updating

Drop a new `index.html` onto the repo (same upload flow). Open `sw.js`, change `mct-v1` to `mct-v2`, commit. The phone picks it up the next time it opens with signal.

## Editing the program

Everything is in `index.html`. The `DRILLS` object holds every drill; the `PLAN` array holds the 8 cycles. Cone positions are in `range()`. Change numbers, save, upload.

## Progress

Stored on the phone (`localStorage`). Cycle screen → **Export progress** copies it as text; paste into **Import** on a new phone.
