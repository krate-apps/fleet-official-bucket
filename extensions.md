# Official Fleet extensions

Catalogue of packages in the [Fleet Official](https://github.com/krate-apps/fleet-official-bucket) bucket (`org.fleet.*`).
Install from **Extensions** in the Fleet UI, or open a repository for details.

| Extension | ID | Description |
| --- | --- | --- |
| [Archive Extract](https://github.com/krate-apps/fleet-ext-archiveextract) | `org.fleet.archiveextract` | Extract .zip and .rar archives under download roots. |
| [Auto Download](https://github.com/krate-apps/fleet-ext-autodownload) | `org.fleet.autodownload` | Watch folders and IRC announces to enqueue magnets and torrents. |
| [Auto Move](https://github.com/krate-apps/fleet-ext-automove) | `org.fleet.automove` | Run label and file actions when torrents finish or change state. |
| [Automation Rules](https://github.com/krate-apps/fleet-ext-automation) | `org.fleet.automation` | Ordered if/then rules for torrents (label, move, throttle, pause, webhooks). |
| [Bandwidth Limits](https://github.com/krate-apps/fleet-ext-bandwidth) | `org.fleet.bandwidth` | Set per-torrent upload and download rate limits on connected clients. |
| [Blocklist](https://github.com/krate-apps/fleet-ext-blocklist) | `org.fleet.blocklist` | Optional peer blocklist from URL lists; kick matching peers when enabled. |
| [Client Logos](https://github.com/krate-apps/fleet-ext-clientlogos) | `org.fleet.clientlogos` | Show peer client logos in the torrent list. |
| [Cookies](https://github.com/krate-apps/fleet-ext-cookies) | `org.fleet.cookies` | Shared per-host cookies for extension HTTP requests. |
| [Cross-seed](https://github.com/krate-apps/fleet-ext-crossseed) | `org.fleet.crossseed` | Push completed downloads to other clients for seeding on the same data path. |
| [Discord](https://github.com/krate-apps/fleet-ext-discord) | `org.fleet.discord` | Notify a Discord channel when torrents are added, finished, or removed. |
| [Disk Cleanup](https://github.com/krate-apps/fleet-ext-diskcleanup) | `org.fleet.diskcleanup` | Report error, stalled, and missing torrents with suggested cleanup actions. |
| [Duplicate Finder](https://github.com/krate-apps/fleet-ext-duplicates) | `org.fleet.duplicates` | Find duplicate torrents across clients; optional hardlink assist. |
| [Event Hooks](https://github.com/krate-apps/fleet-ext-eventhooks) | `org.fleet.eventhooks` | Run allowlisted binaries when torrents are added or finish. |
| [File Manager](https://github.com/krate-apps/fleet-ext-filemanager) | `org.fleet.filemanager` | Browse and manage files under download roots. |
| [File Manager Media](https://github.com/krate-apps/fleet-ext-filemanager-media) | `org.fleet.filemanager-media` | Preview images and run MediaInfo on files under download roots. |
| [File Manager Share](https://github.com/krate-apps/fleet-ext-filemanager-share) | `org.fleet.filemanager-share` | Create share links under download roots with TTL and download limits. |
| [Label Bridge](https://github.com/krate-apps/fleet-ext-labelbridge) | `org.fleet.labelbridge` | Sync labels across registered clients (one-way or bidirectional). |
| [MediaInfo](https://github.com/krate-apps/fleet-ext-mediainfo) | `org.fleet.mediainfo` | Inspect media files with MediaInfo. |
| [Metrics](https://github.com/krate-apps/fleet-ext-metrics) | `org.fleet.metrics` | OpenMetrics endpoint for torrents, clients, disk, and jobs. |
| [NFO](https://github.com/krate-apps/fleet-ext-nfo) | `org.fleet.nfo` | Find and display release NFO files. |
| [NZB Bridge](https://github.com/krate-apps/fleet-ext-nzbbridge) | `org.fleet.nzbbridge` | Turn SABnzbd/NZBGet completed downloads into torrents and enqueue them via Fleet intake. |
| [Notifications](https://github.com/krate-apps/fleet-ext-notifications) | `org.fleet.notifications` | Torrent notifications via ntfy, Gotify, Slack, Pushover, or email. |
| [Port Watch](https://github.com/krate-apps/fleet-ext-portwatch) | `org.fleet.portwatch` | Check whether the torrent listen port stays reachable and alert when it does not. |
| [Post-add Check](https://github.com/krate-apps/fleet-ext-postaddcheck) | `org.fleet.postaddcheck` | Re-announce newly added torrents for a short window. |
| [Public Throttle](https://github.com/krate-apps/fleet-ext-publicthrottle) | `org.fleet.publicthrottle` | Limit upload on public-tracker torrents. |
| [Ratio Colors](https://github.com/krate-apps/fleet-ext-ratiocolors) | `org.fleet.ratiocolors` | Color torrent list rows by ratio thresholds. |
| [Ratio Groups](https://github.com/krate-apps/fleet-ext-ratio) | `org.fleet.ratio` | Enforce ratio and seed-time rules by label. |
| [Ratio Rules](https://github.com/krate-apps/fleet-ext-ratiorules) | `org.fleet.ratiorules` | Assign labels from tracker or privacy rules for Ratio Groups. |
| [Rclone](https://github.com/krate-apps/fleet-ext-rclone) | `org.fleet.rclone` | Copy or move completed downloads to allowlisted rclone remotes. |
| [RSS Feeds](https://github.com/krate-apps/fleet-ext-rssfeeds) | `org.fleet.rssfeeds` | Poll RSS/Atom feeds with filters and enqueue matching items. |
| [RSS Rewrite](https://github.com/krate-apps/fleet-ext-rssrewrite) | `org.fleet.rssrewrite` | Rewrite RSS item download URLs with shared regex rules. |
| [Scheduler](https://github.com/krate-apps/fleet-ext-scheduler) | `org.fleet.scheduler` | Apply weekly bandwidth windows with optional throttle profiles. |
| [Screenshots](https://github.com/krate-apps/fleet-ext-screenshots) | `org.fleet.screenshots` | Extract still frames from video files with ffmpeg. |
| [Servarr Bridge](https://github.com/krate-apps/fleet-ext-servarrbridge) | `org.fleet.servarrbridge` | Receive Sonarr/Radarr/Prowlarr/Lidarr webhooks into Fleet intake. |
| [Spectrogram](https://github.com/krate-apps/fleet-ext-spectrogram) | `org.fleet.spectrogram` | Render audio spectrograms with sox. |
| [Telegram](https://github.com/krate-apps/fleet-ext-telegram) | `org.fleet.telegram` | Notify a Telegram chat when torrents are added, finished, or removed. |
| [Throttle Profiles](https://github.com/krate-apps/fleet-ext-throttle) | `org.fleet.throttle` | Define named throttle profiles and assign them to torrents. |
| [Title Search](https://github.com/krate-apps/fleet-ext-titlesearch) | `org.fleet.titlesearch` | Open external search links from torrent titles. |
| [Torrent History](https://github.com/krate-apps/fleet-ext-history) | `org.fleet.history` | Record when torrents are added, finished, or removed. |
| [Tracker Check](https://github.com/krate-apps/fleet-ext-rutracker_check) | `org.fleet.rutracker_check` | Check tracker topics for updated or deleted torrents. |
| [Tracker Login](https://github.com/krate-apps/fleet-ext-trackerlogin) | `org.fleet.trackerlogin` | Store site credentials and log in to fill the shared cookie jar. |
| [Tracker Replace](https://github.com/krate-apps/fleet-ext-trackerreplace) | `org.fleet.trackerreplace` | Add announce URLs to new or existing torrents. |
| [Traffic](https://github.com/krate-apps/fleet-ext-traffic) | `org.fleet.traffic` | Track upload and download totals by day, month, year, and tracker. |
| [Web Search](https://github.com/krate-apps/fleet-ext-websearch) | `org.fleet.websearch` | Search torrent sites with packaged or custom templates and enqueue results. |
| [XMPP](https://github.com/krate-apps/fleet-ext-xmpp) | `org.fleet.xmpp` | Notify an XMPP contact when a download finishes. |

## Related

- [Coming from Deluge or ruTorrent](coming-from.md)
- [Fleet host](https://github.com/krate-apps/fleet)
