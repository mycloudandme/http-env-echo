node {
  for (int i=0; i< 2; ++i) {
    stage "Stage #"+i
    print 'Hello, world $i!'
  }

  stage "Stage Parallel"
  def branches = [:]
  for (int i = 0; i < 3; i++) {
    branches["split${i}"] = {
      stage "Stage parallel- #"+i
      echo  'Starting sleep'
      sleep 5
      echo  'Finished sleep'
    }
  }
  parallel branches
}

