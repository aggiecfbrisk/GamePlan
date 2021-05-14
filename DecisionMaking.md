# Decision Making
This document defines the process by which the mechanics of the Summer Rust Risk game (hereafter, game), the functionality of the same, and similar matters pertaining to the same may be changed.

## Pre-Game 
- Cosmetic changes only require the approval of any game moderator with pull access to the Risk repository.
- API changes only require the approval of any game moderator with pull access to the Risk repository.
- Mechanical changes must go through the proposal process.
- Security changes must be approved by Mautamu.
- Changes to these rules and other things in this repository are allowed, and each shall be reviewed independently.

## In-Game
- Cosmetic changes only require the approval of any game moderator with pull access to the Risk repository.
- API changes require the approval of at least three game moderators with pull access to the Risk repository.
- Mechanical changes must go through the proposal process.
- Security changes must be approved by Mautamu and at least one other game moderator.
- Changes to these rules and other things in this repository must go through the proposal process.

## Proposal Process
The proposal process is a shortened RFC process, and can be used to change aspects of the game. It follows the following steps/phases:
1. Original requestor (any one may make such a request) submits a pull request (someone may submit a pull request on behalf of other users) against this repository in /proposals/. The recommended proposal format is defined below. 
2. If such a proposal is allowed, any three game moderators may together move the proposal to a Simple Majority User Poll for the next day by approving the PR into /proposals/. Such votes will be conducted on the game platform itself. Ten co-signers (who may simply state "cosign (reddit username)" on the pull request) may do similar. During the game, cosigners must have played at least one turn and not be labeled an alt.


## Definitions
### Cosmetic Changes
A **cosmetic change** is any that is superficial to the game, such as backgrounds, fonts, stylizations, definitions, and the like.
### Application Programming Interface (API) Changes
An **API change** is any change that affects the /api/ of the Rust Risk application interface. Such changes include, but are not limited to: changes to structures, changes to data types, API endpoint additions or removals, and changes to API rules. 
Specifically exempt are any endpoints in the / (root), /auth/ or /docs/ directories. 
### Mechanical Changes
A **mechanical change** is any change that alters the end behavior of the game itself. Most of these mechanical changes pertain either to the /auth/ API endpoints, or to `ringmaster` program.
### Simple Majority User Poll
A **Simple Majority User Poll** is a poll of all users on the game, wherein each team gets a single yes/no/abstain vote. All votes from a team's users are tallied, and then cast as a team vote: yea (50%user+1), nay (50%user-1), or abstain (50%user). Such changes need only a simple majority of teams to approve the change (50%team+1). Abstentions are discarded as non-votes. The process for triggering a poll shall be agreed to in a separate document.
### Pre-Game
The **pre-game** period shall be the period up to and including the first roll. Once the first roll has been made and confirmed by mautamu, the game shall have begun. The [timeline](timeline.md) shall supercede this document in regards to allowing changes.


## Proposal Example
> /proposals/0001-allow-reddit-signin.md

```markdown
# Proposal Title: (Allow Reddit Signin)
Author: Mautamu
Co-Author: Moroniccow
Cosigners: Moroniccow, Jyost17, SomeRedditUser
Request: Change Rust Risk to allow users to signin using Reddit
Linked Pull Request: [5](https://github.com/mautamu/Risk/pull/5) <!-- This can be empty -->

## Rationale
This is necessary to allow people to use the game. This is better than alternatives such as passwords, as it avoids having to store anything locally.

```
