
# AnomaliWeb (Squad Anomali) - Enhanced Prototype

This package is an enhanced prototype tailored to your requests (Squad Anomali).

Key features added:
- Pre-seeded users (IDs 1781..1787) as requested (passwords stored hashed server-side; not revealed in UI).
- Registration flow: users submit registration requests via `/api/register-request` and requests must be approved by an operator via `/api/approve-registration` or the Operator Panel.
- File library with 30 initial folders (can add more, upload files, delete).
- Real-time chat (global public channel + private DM via deterministic channel ids `dm:id1_id2`).
- Online status and online count. Users join personal socket room `user-{id}` for targeted delivery.
- Stickers: upload sticker images (png/jpg/gif/webp) and send as special sticker messages.
- Operator actions: invite/kick/approval events via socket.io (demo flows).
- Basic protections: rate limiting per IP, file size/type checks, sanitized filenames.

How to run:
1. npm install
2. npm start
3. Open http://localhost:4000

Notes:
- Passwords you provided were used to seed users on the server but are NOT exposed in the frontend or registration page.
- This is a prototype. For production, use a proper database, real authentication tokens, HTTPS, and thorough hardening.


-- Updated to v3: UI refreshed (purple+neon), per-user private library endpoints, preview modal, mobile responsive layout.
