<!DOCTYPE html>
<html lang="en">
<body>

<h1>Privacy Policy</h1>

<p><strong>Effective Date:</strong> February 27, 2026</p>

<p>
This Privacy Policy describes how SkyAI (“the Bot”) collects, uses,
and stores information when used within a Valour server.
</p>

<hr>

<h2>1. Information Collected</h2>

<p>
SkyAI collects only the minimum data required to function.
</p>

<h3>Information Stored (In Memory Only)</h3>
<ul>
    <li>Channel IDs</li>
    <li>Message content used for AI conversation context</li>
    <li>Message role (user / assistant / system)</li>
</ul>

<h3>Information Not Stored</h3>
<ul>
    <li>Direct Messages (DMs)</li>
    <li>User credentials</li>
    <li>Email addresses</li>
    <li>Passwords</li>
    <li>IP addresses</li>
    <li>Analytics or tracking data</li>
</ul>

<p>
Conversation history exists only in memory and is erased when the bot restarts
or when the <code>s.cm</code> command is used.
</p>

<hr>

<h2>2. Purpose of Data Collection</h2>

<p>Stored information is used exclusively to:</p>

<ol>
    <li>Maintain conversational context within a channel</li>
    <li>Generate AI responses using prior messages</li>
    <li>Enable core bot command functionality</li>
</ol>

<p>
Data is not used for marketing, advertising, profiling, or analytics.
</p>

<hr>

<h2>3. Data Storage and Security</h2>

<p>
All data is stored temporarily in RAM on the hosting server.
</p>

<p>
No conversation data is persisted to disk by default.
</p>

<p>
The operator of the self-hosted instance is responsible for
securing the hosting environment.
</p>

<hr>

<h2>4. Third-Party Processing</h2>

<p>
SkyAI forwards message content to a self-hosted AI backend
via Open WebUI.
</p>

<p>
Depending on configuration, this may include:
</p>

<ul>
    <li>Ollama (local model execution)</li>
    <li>Other self-hosted LLM providers configured by the operator</li>
</ul>

<p>
SkyAI does not transmit data to external cloud AI providers
unless explicitly configured by the host operator.
</p>

<hr>

<h2>5. Data Retention</h2>

<p>
Conversation data is retained only during runtime.
</p>

<p>
Data is removed when:
</p>

<ul>
    <li>The bot process stops</li>
    <li>The bot restarts</li>
    <li>The <code>s.cm</code> command is executed</li>
</ul>

<hr>

<h2>6. Self-Hosted Responsibility</h2>

<p>
SkyAI is designed for self-hosting.
</p>

<p>
The hosting operator is responsible for:
</p>

<ul>
    <li>Server security</li>
    <li>Network configuration</li>
    <li>API key protection</li>
    <li>Compliance with applicable laws</li>
</ul>

<hr>

<h2>7. Changes to This Policy</h2>

<p>
If data collection practices change in future versions,
this Privacy Policy will be updated prior to implementation.
</p>

<p>
Continued use of the Bot after updates constitutes acceptance
of the revised policy.
</p>

<hr>

<h2>8. Contact Information</h2>

<p>
For privacy-related inquiries:
</p>

<p>
Email: contact@skyjoshua.xyz
</p>

</body>
</html>