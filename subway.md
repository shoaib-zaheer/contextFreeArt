startshape subway

shape section
  rule 1000 {
            CIRCLE []
            section [y 0.1]
}
//terminal
rule 1{
      CIRCLE[s 3]
      CIRCLE[s 1 b 1]
}

// add turns

rule 1{section [r 45]}
rule 1{section [r -45]}
rule 1{section [r 90]}
rule 1{section [r -90]}

//add stops

rule 4 {
        SQUARE [s 3 r 45]
        section []
}


rule 0.45{

  section []
  // call anther line
  // perpendicular to the current one
    subway [rotate 90]
}


shape subway 
  
    rule {
          section [b 0.7 sat rand (1, -1) hue rand(20, -10) ]
          section [b 0.7 sat rand (1, -1) hue rand(20, -10) rotate 180]
                    section [b 0.7 sat rand (1, -1) hue rand(20, -10) rotate 180]
}
/*
x sin (i * 0.95)
y cos (i * 1)
][]*/
