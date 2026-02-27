<!DOCTYPE html>
<html lang="en">
<body>

<h1>SkyAI</h1>

<p>
SkyAI is a Valour.gg bot powered by a self-hosted Large Language Model via Open WebUI.
</p>

<p>
It supports per-channel conversational memory and is designed for self-hosted deployments.
</p>

<hr>

<h2>Features</h2>
<ul>
    <li>Per-channel AI conversation history</li>
    <li>Self-hosted LLM support (Open WebUI + Ollama)</li>
    <li>Built with .NET</li>
    <li>Open-source under AGPL-3.0</li>
    <li>Privacy-conscious architecture</li>
</ul>

<hr>

<h2>How It Works</h2>
<p>SkyAI connects to:</p>
<ul>
    <li>Valour.gg API</li>
    <li>Open WebUI <code>/api/chat/completions</code> endpoint</li>
    <li>A locally hosted LLM (e.g., llama3.1 via Ollama)</li>
</ul>

<p>
Conversation history is stored in memory per channel and sent with each request
to maintain contextual awareness. History is automatically trimmed to prevent
excessive token usage.
</p>

<hr>

<h2>Data &amp; Privacy</h2>

<p>SkyAI stores only the minimum data required for operation.</p>

<h3>Stored In Memory (Per Channel)</h3>
<ul>
    <li>Channel ID</li>
    <li>Message content (AI conversation context only)</li>
    <li>Message role (user / assistant / system)</li>
</ul>

<h3>Not Stored</h3>
<ul>
    <li>Direct Messages</li>
    <li>User credentials</li>
    <li>Email addresses</li>
    <li>Analytics or tracking data</li>
</ul>

<p>
Conversation history resets automatically when the bot restarts.
</p>

<p>
Full privacy policy:<br>
<a href="https://github.com/SkyJoshua/SkyAI/blob/main/PRIVACY.md">
https://github.com/SkyJoshua/SkyAI/blob/main/PRIVACY.md
</a>
</p>

<hr>

<h2>License</h2>
<p>
This project is licensed under the
<strong>GNU Affero General Public License v3.0 (AGPL-3.0)</strong>.
</p>

<p>
See the LICENSE file for details:<br>
<a href="https://github.com/SkyJoshua/SkyAI/blob/main/LICENSE">
https://github.com/SkyJoshua/SkyAI/blob/main/LICENSE
</a>
</p>

<p>
If you modify and deploy this project publicly (including as a hosted service),
you must make your source code available under the same AGPL-3.0 license.
</p>

<hr>

<h2>Installation</h2>

<pre><code>git clone https://github.com/YOUR_USERNAME/SkyAI.git
cd SkyAI
dotnet restore</code></pre>

<p>
All required NuGet packages are installed automatically via <code>SkyAI.csproj</code>.
</p>

<hr>

<h2>Requirements</h2>
<ul>
    <li>.NET 8+</li>
    <li>Open WebUI running</li>
    <li>Ollama running with a model (e.g., llama3.1)</li>
    <li>Valid Valour bot token</li>
</ul>

<hr>

<h2>Configuration</h2>

<p>Create a <code>.env</code> file in the root directory:</p>

<pre><code>TOKEN=your-valour-bot-token
OPENWEBAPI=your-openwebui-api-key
OPENWEBURL=your-openwebui-url</code></pre>

<p>
Do not commit this file to version control.
</p>

<hr>

<h2>Running the Bot</h2>

<pre><code>dotnet run</code></pre>

<hr>

<h2>Commands</h2>

<table border="1" cellpadding="6">
<tr>
<th>Command</th>
<th>Description</th>
</tr>
<tr>
<td><code>s.ai &lt;message&gt;</code></td>
<td>Send a prompt to the AI</td>
</tr>
<tr>
<td><code>s.cm</code></td>
<td>Clear channel conversation memory</td>
</tr>
<tr>
<td><code>s.source</code></td>
<td>Shows the source code of the bot</td>
</tr>
</table>

<hr>

<h2>Self-Hosting Notes</h2>

<p>Ensure Ollama is running:</p>

<pre><code>ollama serve</code></pre>

<p>Ensure your model is installed:</p>

<pre><code>ollama list</code></pre>

<hr>

<h2>Contributing</h2>

<p>
Contributions are welcome. By submitting a contribution, you agree that your
contributions will be licensed under AGPL-3.0.
</p>

<ol>
    <li>Fork the repository</li>
    <li>Create a feature branch</li>
    <li>Submit a pull request</li>
</ol>

</body>
</html>