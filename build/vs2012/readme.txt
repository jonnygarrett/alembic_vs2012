--------------------------------------------------------------------------------
alembic 1.1.5 vs2012 x64
--------------------------------------------------------------------------------

copy vs2012 folder to build\vs2012


setup contrib libraries:

  ilmbase-1.0.2
    http://download.savannah.nongnu.org/releases/openexr/ilmbase-1.0.2.tar.gz
    extract to contrib\ilmbase-1.0.2
    
    copy build\vs2012\contrib\toFloat.h to contrib\ilmbase-1.0.2\Half\toFloat.h
    copy build\vs2012\contrib\eLut.h    to contrib\ilmbase-1.0.2\Half\eLut.h

  openexr-1.6.1
    http://download.savannah.nongnu.org/releases/openexr/openexr-1.6.1.tar.gz
    extract to contrib\openexr-1.6.1

  hdf5-1.8.9
    prebuilt x64 binaries from
      http://www.hdfgroup.org/ftp/HDF5/releases/hdf5-1.8.9/bin/windows/HDF5189-win64-vs10-static.zip
    extract HDF5189-win64-vs10-static.zip
    extract HDF5-1.8.9-win64.exe (using 7zip)
    copy contents of $_OUTDIR (bin, include, lib, share) to contrib\hdf5-1.8.9-win64

  zlib-1.2.8
    http://zlib.net/zlib-1.2.8.tar.gz
    extract to contrib\zlib-1.2.8
    
  glew-1.9.0
    prebuilt x64 binaries from
      https://sourceforge.net/projects/glew/files/glew/1.9.0/glew-1.9.0-win64.zip/download
    extract to contrib\glew-1.9.0

  glut-3.7.6
    prebuilt x32 and x64 binaries from
      http://www.idfun.de/glut64/glut-3.7.6-bin-32and64.zip
    extract to contrib\glut-3.7.6-bin\gl
    (ie. glut-3.7.6-bin\gl contains glut.h and the libs / dlls)


build in visual studio

