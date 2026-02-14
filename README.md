PingMaster: Real-Time Network Diagnostics

App Description

PingMaster is a high-performance network diagnostic tool designed to provide real-time insights into connection stability and latency. By utilizing recurring HTTP-based requests to a user-defined target URL, the application calculates precise round-trip times (RTT) and visualizes network performance through a dynamic, high-frequency stability chart.

Whether you are troubleshooting a slow ISP connection, testing server responsiveness, or monitoring long-term network health, PingMaster offers an intuitive interface to decode complex network behavior. The app categorizes results with smart quality badges—ranging from "Better" for peak performance to "Bad" for high-latency scenarios—allowing users to identify network jitter, micro-stutters, and potential bottlenecks at a glance.

Key Features

Real-Time Latency Tracking: Visualizes every ping attempt on a responsive line chart.

Categorized Quality Indicators: Instant feedback with descriptive badges:

Better (< 50ms): Ideal for gaming and real-time communication.

Good (50ms - 150ms): Smooth web browsing and streaming.

Poor (150ms - 300ms): Noticeable lag in interactive applications.

Bad (> 300ms): High latency, likely to cause significant delays.

Statistical Aggregates: Automatically calculates Session Average, Minimum, and Maximum latency.

Adjustable Intervals: Choose between Fast (500ms), Normal (1s), and Slow (3s) polling frequencies.

Live Diagnostic Log: A scrollable history of connection attempts with timestamps and status reports.

Network Presets: One-click configurations for major backbones like Google, Cloudflare, and GitHub.

Technical Details

HTTP vs. ICMP

Standard browser security (sandboxing) prevents JavaScript from sending raw ICMP "Echo Request" packets (traditional ping). PingMaster overcomes this by measuring the timing of an asynchronous fetch request. To ensure accuracy:

Cache Busting: Uses cache: 'no-store' to force the network to fetch a fresh response rather than pulling from local memory.

CORS-Agnostic: Implements mode: 'no-cors' to allow timing measurements even if the target server does not explicitly allow cross-origin resource sharing.

Getting Started

Target URL: Enter the URL you wish to test (e.g., https://www.google.com).

Interval: Select how frequently you want to poll the server.

Start Testing: Click the blue button to begin the diagnostics.

Monitor: Observe the "Current" stat and the "Stability Graph" for fluctuations (jitter).

Clear Log: Use the clear button if you wish to reset the history for a new test session.

Developed as a modern web-based utility for network administrators, developers, and power users.
