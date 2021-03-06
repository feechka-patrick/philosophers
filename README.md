# philosophers
RUN : make
<br>
./philo [number of philo] [time_to_die] [time_to_eat] [time_to_sleep] [(optional) number_of_times_each_philosopher_must_eat]]
<br>
<br>

ПОСТАНОВКА ЗАДАЧИ: 
<br>Пять безмолвных философов сидят вокруг круглого стола, перед каждым философом стоит тарелка спагетти. Вилки лежат на столе между каждой парой ближайших философов.
<br>Каждый философ может либо есть, либо размышлять. Приём пищи не ограничен количеством оставшихся спагетти — подразумевается бесконечный запас. Тем не менее, философ может есть только тогда, когда держит две вилки — взятую справа и слева (альтернативная формулировка проблемы подразумевает миски с рисом и палочки для еды вместо тарелок со спагетти и вилок).
<br>Каждый философ может взять ближайшую вилку (если она доступна) или положить — если он уже держит её. Взятие каждой вилки и возвращение её на стол являются раздельными действиями, которые должны выполняться одно за другим.
<br>Вопрос задачи заключается в том, чтобы разработать модель поведения (параллельный алгоритм), при котором ни один из философов не будет голодать, то есть будет вечно чередовать приём пищи и размышления.

TEST : 
  - Test with ./philo 1 800 200 200, the philosopher should not eat and should die
  - Test with ./philo 5 800 200 200, no one should die
  - Test with ./philo 5 800 200 200 7, no one should die and the simulation should stop when all the philosopher has eaten atleast 7 times each
  - Test with ./philo 4 410 200 200, no one should die
  - Test with ./philo 4 310 200 100, a philosopher should die

