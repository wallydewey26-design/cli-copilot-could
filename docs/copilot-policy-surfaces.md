# Copilot policy applicability by surface

The following table shows which surfaces each Copilot policy applies to.
A policy cell marked **✓** means an admin or organization owner can govern
that feature on that surface through the policy.
A cell marked **—** means the policy does not apply to that surface - either
because the underlying feature is unavailable there, or because the surface
falls outside the policy's scope.

> **Note:** This table describes whether a policy *controls* a feature on a
> surface, not whether the feature *exists* on that surface. A "—" entry does
> not necessarily mean the feature is absent everywhere - it means the policy
> has no effect on that particular surface.

## Policy applicability table

| Policy | IDEs | Copilot Chat on GitHub | Cloud agent | CLI |
|---|:---:|:---:|:---:|:---:|
| Copilot can search the web | ✓ | ✓ | — | — |
| MCP servers in Copilot | ✓ | — | ✓ | ✓ |

### Notes on specific policies

**Copilot can search the web**
Web search is available in IDEs and Copilot Chat on GitHub, so the policy
controls it on those two surfaces. Web search is not available in the cloud
agent or the CLI; the policy therefore does not apply to those surfaces (marked
—).

**MCP servers in Copilot**
MCP server support exists in IDEs, the cloud agent, and the CLI, so the policy
governs those surfaces. MCP servers are not available in Copilot Chat on
GitHub; the policy therefore does not apply there (marked —).

## Feature availability vs. policy applicability

These are two separate questions:

| Question | Answered by |
|---|---|
| Does this feature exist on this surface? | Feature availability matrix |
| Can an admin turn this feature on or off for this surface? | Policy applicability table (this document) |

When a feature is available on a surface but no policy controls it, admins
cannot toggle it - it is always on for users on that surface. When a feature
is unavailable on a surface, the policy has no surface to act on, so the
cell is also marked —.
