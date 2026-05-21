# zmk-config

Этот репозиторий содержит пользовательскую конфигурацию ZMK для split-клавиатуры Mriya.

## Что собирается

- Левая половина: `mriya_left`
- Правая половина: `mriya_right`
- Донгл Prospector: официальная плата `nice_nano` + щит `settings_reset`

## Как работает сборка

GitHub Actions использует `./.github/workflows/build.yml` и `build.yaml`.
Конфигурация `config/west.yml` подключает официальную ветку ZMK через `app/west.yml`, а `build.yaml` задаёт матрицу сборки.

## Сохранение раскладки

Оригинальная раскладка сохраняется в `config/mriya.keymap` и подключается из `config/boards/arm/mriya/mriya_left.keymap` и `config/boards/arm/mriya/mriya_right.keymap`.
