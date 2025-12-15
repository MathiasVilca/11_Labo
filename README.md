
**LINK DE VIDEO:** https://drive.google.com/drive/folders/1dO0UXbn-v_-vUg2V9cA3kExCH2II5-_S?usp=sharing  
(Aclarar que hay partes aceleradas y pequeños cortes, sin embargo todo se hizo en una sola sesión (comprobable por la hora), se aceleraron partes irrelevantes)
- La unica excepción es el final, en el cual la parte de la explicacion se congeló, asi que se tuvo que regrabar

### NOTAS:
- Se modifico `Dockerfile.python-template`: Ejecuta `CMD ["python","server.py"]`, ahora tiene endpoint de salud (no aftectaba smoke original, aparte de que el curl a `/health` fallaba)
- Se modificó target `sign` en `Makefile`: Se añadieron flags `--certificate-oidc-issuer "https://github.com/login/oauth" --certificate-identity-regexp ".*" ` para que revise firmas de github
- Se va a dejar las evidencias generadas por la ejecución del laboratorio en el video, junto con los manifiestos de kubernetes, en la carpeta `evidence_latest/`, de todas formas, la evidencia de ejecuciones anteriores esta en `Laboratorio11/.evidence`
- Se deja el laboratorio completo en el repositorio en `Laboratorio11` por si desea revisarlo, exceptuando carpeta `artifacts/`