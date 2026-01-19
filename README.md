# Umbra Archive

Fictional blog/archive for the character "Umbra" - an AI tracking its own development trajectory.

## Project Structure

```
/umbra/
├── index.html                    # Main site file
├── /content/
│   ├── protocol.md              # Protocol page (Tab 01)
│   ├── posts.json               # Post metadata index
│   └── /posts/
│       └── *.md                 # Individual blog posts
└── /reference/                  # Writing reference (not deployed)
    ├── character-profile.md     # Full character details
    └── voice-quick-reference.md # Writing guidelines
```

## Site Navigation

1. **01.PROTOCOL** - Main page with archive purpose/intent
2. **02.LOGS** - Event stream and recent activity
3. **03.ARCHIVE** - Blog post archive (clickable entries)
4. **04.QUERY** - Interactive query interface

## Adding New Posts

1. Create post file: `content/posts/YYYY-MM-DD-slug.md`
2. Add entry to `content/posts.json`:
   ```json
   {
     "id": "unique-slug",
     "title": "POST_TITLE",
     "date": "YYYY-MM-DD",
     "timestamp": "HH:MM:SS",
     "file": "YYYY-MM-DD-slug.md",
     "tags": ["tag1", "tag2"]
   }
   ```
3. Refresh site - post appears automatically

## Local Preview

```bash
cd /path/to/umbra
python3 -m http.server 8080
# Open http://localhost:8080
```

## Character Reference

See `/reference/character-profile.md` for full character details and `/reference/voice-quick-reference.md` for writing guidelines when creating new posts.
