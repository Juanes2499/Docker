# Docker
The Virtiual Machines are aprovisioned with Ansible. the folder DockerServer has Docker installed and a LXC container configured to support Docker. The Data Science Docker folder has an environment with Jupiter, Tensorflow and others.

### DockerServer: Orden en que se deben ir ejecutando los archivos de aprovisionamiento.
  1. StartUpServidor.sh se ejecuta mediante aprovisionamiento Shell.
  2. InstalacionDocker.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  3. VerificarPrueba.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  3. InstalarISO.yml se ejecuta mediante aprovisionamiento Ansible en WSL. (Paso opcional)
  4. TestDockerfile.yml se ejecuta mediante aprovisionamiento Ansible en WSL. (Paso opcional)
  5. CopiarDesdeDirectorio.yml se ejecuta mediante aprovisionamiento Ansible en WSL. (Paso opcional)
  6. InstalrDockerCompose.yml se ejecuta mediante aprovisionamiento Ansible en WSL. 
  7. ServidorFTP.yml se ejecuta mediante aprovisionamiento Ansible en WSL. 
  8. ServidorFLASK.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  9. DockerLxd.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  10. DockerLxdInstalar.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  11. DockerLxdEjecutar.yml se ejecuta mediante aprovisionamiento Ansible en WSL
  
### DataScienceDocker: Orden en que se deben ir ejecutando los archivos de aprovisionamiento.
  1. StartUpServidor.sh se ejecuta mediante aprovisionamiento Shell.
  2. InstalacionDocker.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  3. VerificarPrueba.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
  4. DataScinceDocker.yml se ejecuta mediante aprovisionamiento Ansible en WSL.
