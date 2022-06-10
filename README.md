<h1>Technologie Chmurowe - Laboratorium 13B</h1>
<h2>Autor: Michał Moń</h2>
<h3>Opis repozytorium:</h3>
W repozytorium znajdują się foldery <b>nginx-old</b> oraz <b>nginx-new</b>, które zawierają pliki Dockerfile oraz index.html służące do zbudowania obrazów <b>"nginx-old"</b> oraz <b>"nginx-new"</b>, które zostały wypchnięte do repozytorium Dockerhub (<a href="">Link</a>). Obrazy te bazują na "klasycznym" obrazie serwera "nginx", jednakże domyślny plik "index.html" widoczny po uruchomieniu został zastąpiony własnym plikiem <b>"index.html"</b>, który wyświetla wersję aktualnie uruchomionego serwera "nginx".<br/><br/>
Ponadto zostały przygotowane 4 pliki <b>nginx-deployment-v1/v2/v3/v4.yml</b>, każdy z nich realizuje kolejny z etapów założonych w zadaniu:
<ul>
  <li><b>nginx-deployment-v1.yml</b> - wdrożenie usługi, liczba replik: 3, obraz: nginx-old</li>
  <li><b>nginx-deployment-v2.yml</b> - zwiększenie liczby replik, liczba replik: 6, obraz: nginx-old</li>
  <li><b>nginx-deployment-v3.yml</b> - zmiana obrazu na nginx-new, liczba replik: 6, obraz: nginx-new </li>
  <li><b>nginx-deployment-v4.yml</b> - ustawienie limitów zasobów, liczba replik: 6, obraz: nginx-new</li>
</ul>
