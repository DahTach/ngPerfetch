# ngPerfetch
Angular PWA SOTA Fetching Techniques

## Strategy
- Prefetching
- Caching
- Background Syncing
- Offline First
- Lazy Loading
- Client-Side Rendering

## Storage
- In Memory
- Cache API ( Service Worker )
- IndexedDB
- LocalStorage

## Use Cases

### Cache API - Asynchronous
- Assets (JS, CSS, images, fonts)
- Network request/response pairs
- Offline access to network resources
- Improves load performance via cached resources
Persistent until cleared or cache expires (managed by Service Worker)

### IndexedDB - Asynchronous
- Large amounts of structured data
- Data requiring indexing or complex querying (cursors)
- Offline storage of application data
- Binary data (Files/Blobs)
- Large data volumes
Persistent until explicitly cleared (by user or application or system); largest potential storage

### LocalStorage - Synchronous
- Small amounts of simple key-value data (strings)
- User preferences (e.g., theme, language)
- Simple application settings or flags
- Remembering simple states across sessions
Persistent until explicitly cleared (by user or application); small size limit (typically 5-10MB)
