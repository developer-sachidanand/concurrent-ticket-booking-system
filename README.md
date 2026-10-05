# Concurrent Ticket Booking System

A high-performance concurrent ticket booking system built in Go, designed to handle high-volume user traffic and prevent double-booking using thread-safe data structures and synchronization primitives.

---

## Features

- **High Concurrency Handling:** Leverages Go's goroutines and channels to process a large volume of simultaneous booking requests efficiently.
- **Race Condition Prevention:** Utilizes thread-safe synchronization primitives (such as `sync.Mutex` / atomic operations) to ensure seat availability is accurate and prevent overbooking/double-booking.
- **Web Frontend:** Simple web interface provided via HTML/CSS static files to simulate user seat selection and real-time booking updates.
- **Docker Support:** Includes `docker-compose` setup for quick deployment and local development.

---

## Project Structure

```text
.
├── cmd/                # Application entry points / main packages
├── internal/           # Private application code (booking logic, concurrency handlers)
├── static/             # Static web assets (HTML, CSS, JavaScript)
├── docker-compose.yaml # Container orchestration setup
├── go.mod              # Go module definition
└── go.sum              # Go module checksums