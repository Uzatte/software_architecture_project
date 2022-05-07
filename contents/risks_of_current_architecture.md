### Анализ рисков созданной архитектуры, компромиссов

**Распределенная архитектура**

Несмотря на то, что распределенная архитектура на основе микросервисов предоставляет ряд неоспоримых преимуществ, в то же время она является серьезным компромиссом и источником ощутимых рисков.

Главным компромиссом данной стиля является производительность, которая деградирует с каждым запросом проходящим по сети.
Сеть же, является одним из самых существенным факторов риска, т.к. ее недоступность на любом сегменте взаимодействия самым существенным образом скажется на доступности и производительности системы.

**PaaS платформа**

С одной стороны PaaS платформа снимает с нас колоссальный объем работы в плане развертывания и обслуживания инфраструктуры, но с другой стороны крайне сильно завязывает наше приложение на поставщике услуг и делает нас зависимым от него, накладывая по сути vendor-lock. Так же, все наши данные, в т.ч. и чувствительные, хранятся на сторонних серверах, и мы можем уповать только на профессионализм и порядочность поставщика.

**Риски безопасности**

Созданная архитектура пытается минимизировать, но не может исключить риски связанные с безопасность, в т.ч. безопасностью персональных данных пользователей и потенциальных возможностей их утечки.

**Риски связанные с использованием открытого ПО**

В связи с текущей геополитической ситуации приложение будет стараться максимально использоваться открытое ПО, чтобы не попасть под потенциальные санкции коммерческих компаний. Однако, использование открытого ПО несет в себе риски связанные с недобросовестными разработчиками, которые могут добавить в свои пакеты закладки или вредоносный код. 

