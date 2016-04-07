stage 'Checkout'
node {
  checkout scm

  for (int i=0; i<2; i++) {
    stage "Stage Build #$i"
    print "Hello, world $i!"
    sh 'ls -l'
  }
  stage 'post'
  print "Goodbye"
}

