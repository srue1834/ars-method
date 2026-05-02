## Metodología - Git y GitHub

1. Creo repositorio en [Github](https://github.com)<br>

2. Creo carpeta "ars-methodi" y me adentro con la terminal `cd ...url/ars-methodi`<br>

3. `git init`<br>

4. Creo archivo examen.md y traigo: [Examen](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-examen-md)<br>

5. `git status`<br>

6. `git add .`<br>

7. `git status`<br>

8. `git commit -m "usuario_upv: Añado información del examen"`<br>

9. `git log --oneline`<br>

10. `git remote add origin https://. . .`<br>

11. `git push -u origin main`<br>

12. Explicar lo del [PAT](https://gist.github.com/fernanCordon/f97842efad7269edb258ab528053b87c)<br>

13. Creo archivo evolutio.md y traigo: [Evolutio](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-evolutio-md)<br>

14. `git status`<br>

15. `git add .`<br>

16. `git commit -m "usuario_upv: Añado metodología de trabajo"`<br>

17. `git checkout -b experimento-1`<br>

18. Borro cosas, añado otro archivo, añado carpeta con un archivo dentro, modifico lo que quiera...<br>

19. `git checkout -- .`<br>

20. Elimino los archivos y carpetas que no necesito.<br

21. Vuelvo a hacer cambios<br>

22. `git add .`<br>

23. `git commit -m "tuUsuario: He cambiado el diseño"`<br>

24. `git push -u origin experimento-1`<br>

25. Sigo haciendo cambios...<br>

26. `git add .`<br>

27. `git commit -m "tuUsuario: Añado funcionalidad X"`<br>

28. `git push origin experimento-1`<br>

29. `git checkout main`<br>

30. `git log --oneline --all --graph --decorate`<br>

31. Creo archivo revisio.md y traigo: [Revisio](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-revisio-md)<br>

32. Creo archivo proiectum.md y traigo:[proiectum](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-proiectum-md)<br>

33. `git status`<br>

34. `git add .`<br>

35. `git status`<br>

36. `git commit -m "tuUsuario: Modifico este proyecto"`<br>

37. `git push origin main`<br>

38. `git log --oneline --all --graph --decorate`<br>

39. Copio el hash del primer commit (de la rama main)<br>

40. `git checkout -b experimento-2 a1b2c3d` (hash del commit primero)<br>

41. Cambio y añado cosas<br>

42. `git add .`<br>

43. `git commit -m "tuUsuario: modifico lo que sea…"`<br>

44. `git push -u origin experimento-2`<br>

45. `git checkout main`<br>

46. Creo archivo comandos.md y pego: [Comandos](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-comandos-md)<br>

47. Creo archivo sequentia.md y pego: [Sequencia](https://gist.github.com/fernanCordon/4d00562773340e0a0817e31646be133b#file-vue-git-sequentia-md)<br>

48. `git add .`<br>

49. `git commit -m "tuUsuario: modifico lo que sea…"`<br>

50. Creo archivo PAT.md y pego: [PAT](https://gist.github.com/fernanCordon/f97842efad7269edb258ab528053b87c)<br>

51. `git add .`<br>

52. `git commit -m "tuUsuario: modifico lo que sea…"`<br>

53. `git push origin main`<br>

54. `git log --oneline --all --graph --decorate`<br>