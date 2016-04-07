node {
  stage 'Checkout'
  checkout scm

  for (int i=0; i<2; i++) {
    stage "Stage Build #"+i
    print 'Hello, world $i!'
  }
}

