
.. _trunkGroup-name:

Name
----

| Trunk group name.




.. _trunkGroup-type:

Type
----

| Type.
| It's how the system will sort the trunk that belongs to a group.
| 
| * In order. The system will send a call to the trunks that are in the selected order
| * Random. The system will sort the trunks in a randomized manner, using the RAND() function of MYSQL, therefore, will be able to repeat the trunk in sequence.
| * LCR. Sorth the trunks that have a lower cost. If the trunk owner does not have tariff, will be desconsidered and will be put it in last. 
| 
| MagnusBilling will send the calls to the trunks that belongs in this group, until the calls are answered, occupied or canceled.
| 
| MagnusBilling will try to send the calls to the next trunk of the group as long as the next tested trunk group answer CHANUNAVAIL or CONGESTION, these are the values returned by Asterisk, and it's not possible to change.
| 
| 
| 
| 




.. _trunkGroup-id-trunk:

Trunk
-----

| Select the trunks that belongs to this group. If selected the type, order, then select the trunks in the desired order.



