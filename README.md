# horus-live-url

A one-file pointer repo. `url.txt` holds the current public tunnel URL for
the hosted Horus clone — nothing else lives here on purpose.

Written by `tools/horus-host/reapply-url.mjs` (in the `starfleet-development`
repo) on every tunnel rotation. Read by Fleet-Com's `/horus` redirect
(`fleet-com/app/horus/route.ts`) via the raw GitHub content URL, cached
briefly. This repo is intentionally decoupled from the software repos it
serves — it is operational pointer data, not source, and rotates far too
often to belong in either repo's own commit history.

Public and unauthenticated by design: the URL it holds is, by definition,
already reachable by anyone who has it.
