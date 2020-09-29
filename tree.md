startshape tree


shape tree 
rule 1// regular stem section 

{
SQUARE []
tree [y 1 s 0.99 r 1.5]
}

rule 0.1 // change curve direction 
{
tree [flip 90]
}
 rule 0.05// spawn branches
   {
 tree [s 0.99 r 1.5 flip 90]
  tree [s 0.6 x 0.5 r -60]
   tree [s 0.6 x-0.5 r 60]
 }
 
  rule 0.005// spawn branches
   {
 CIRCLE [s rand (5, 30) a rand (2, -1)]

 }

