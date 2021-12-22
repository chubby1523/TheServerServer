# Land Claiming and Grief Protection
Our server uses the [grief prevention](https://dev.bukkit.org/projects/grief-prevention) plugin to manage land claiming and grief protection
## Land Claims
?>**Land claims** are areas where a player has control over who can build, access chests and other settings in their land claim, this helps prevent grief and protects not only your builds but also your chests and items!
### Creating land claims
#### Creating claims from scratch
- Your first land claims is an automatically generated **9x9 square** around the first chest you place! This helps protect new players!

To create a land claim, a **golden shovel** is required:
1. Right click with a **golden shovel** on a block which will act as a corner of your land claim
2. **Without switching to any other item** locate the other corner of your land claim and right click on that block
3. A rectangular land claim will be generated.

!> Abusing the land claiming system is strictly prohibited and players who claim an excessive amount of land will be punished. See [Server Rules](/serverrules.md) for more details.

#### Resizing an existing claim
1. Start by **right clicking** land in your claim with a stick. This will show you your land claim. See more [here](#With-a-stick-in-game).
2. Right click a corner of your claim with a **golden shovel**.
3. **Without switching to any other item** locate the new corner of your claim and right click that block.
4. Your land claim will have been resized.


#### Creating Subdivisions
Subdivisions allow a claim to be split up into **different areas** with **different permissions**, this is useful if you need to have a super secure part of your base, but want to let other people explore the rest of it. To make a subdivision:
1. Stand in the claim you want to subdivide and use `/SubdivideClaims` to switch your golden shovel into subdivision mode.
2. Locate one corner of your subclaim and right click it with the golden shovel.
3. **Without switching to any other item** locate the other corner of your new subdivision and right click that block.
4. A new subclaim will have been made, use `/RestrictSubclaim` to remove the permissions it inherited from the parent claim. Then, stand inside the subclaim and use commands to give permissions specifically for that subclaim.

#### Viewing your claim
>There are two ways to view your claim, with the **server map** or in game with a **stick**.
##### On the server map
1. Open the [server map](http://tools.server.alexmiao.com:8123/).
2. Hover over the layers panel(top left) and tick **Claims**.
3. Player claims will show on the map as red boxes, click on the claims to show claim owners.

?>The server map updates claims in near **real time** meaning players can adjust their claims while watching the server map to get a better understanding of the land they are claiming. See [The Server Map](/servermap.md) for more details.

![](_media\claimsonmap.png)</br>*@Joshua8Chan's land claim*
##### With a stick in game
- Right clicking with a stick on a land claim shows you *who claimed that land* and also displays *the boundaries of that claim* as glowstone in game.

![bounderies of a claim](_media\landclaimingame.png) *In game bounderies of a land claim when right clicked with a stick*

### Managing land claims
!>Never give someone you don't trust full permissions in your claim. This is **your** responsibility, not the server admin's.

Players can manage their land claim by issuing commands while standing in the claim/subclaim.

?> When giving permissions, players can give permissions to `all` to give all players permissions. e.g. `/accesstrust all` will allow all players to use just buttons, levers and beds in your claim.

`/AbandonClaim` - Deletes the claim you're standing in.</br>
`/Trust` - Gives another play full permissions in your claim except for editing permissions.</br>
`/UnTrust` - Revokes any permissions granted to a player in your claim.</br>
`/AccessTrust` - Gives a player permission to use your buttons, levers and beds.</br>
`/ContainerTrust` - Gives a player permission to use your buttons, levers, beds, crafting gear, containers (e.g. chests) and animals.</br>
`/TrustList` - Lists all the permissions of different players in the claim you're standing in.</br>
`/SubdivideClaims` - Switches your shovel to subdivision mode, so you can subdivide your claims.</br>
`/RestrictSubclaim` - Restricts a subclaim, so that it inherits no permissions from the parent claim.</br>
`/BasicClaims` - Puts your shovel back in basic claims mode.</br>
`/AbandonAllClaims` - Deletes all of your claims.</br>
`/ClaimsList` - Lists a player's claims and claim block details.</br>
`/Trapped` - If you are trapped inside a claim, use this to get unstuck.</br>
`/PermissionTrust` - Grants a player permission to share his permission level with others. e.g. if a player has access trust and you give them permission trust, they are able to give others access trust.</br>