# Anti-SandboxBOF-SLIVERC2
🧪 sandbox-process

Author: yan16-DZ

Original author: Gabriel Landau (Elastic)

Sliver extension — Windows x64

🛡️ Description
sandbox-process is an extension for the Sliver C2 framework that allows dynamically modifying the security level of a target process by stripping its privileges and assigning it an Untrusted token.
This technique is useful in sandbox detection contexts, where "non-privileged" behavior is typically ignored by behavioral security solutions (EDR/Sandbox).

🎯 Purpose
Enables red team operators and pentesters to:

Remove sensitive privileges from a process token (e.g., SeDebugPrivilege)

Set the integrity level to Untrusted for a running process

Simulate sandbox evasion behavior to identify automated detection environments

⚙️ Features
Strips privileges from the token of the specified process

Changes the integrity level to Untrusted

Requires the coff-loader to be loaded in Sliver

📦 Structure

🎯 PID required: target process ID

🧱 Architecture: Windows x64

🔗 Dependency: coff-loader

🧠 Inspiration
This module is inspired by the work of Gabriel Landau (Elastic) on Untrusted tokens and sandbox bypass techniques.
