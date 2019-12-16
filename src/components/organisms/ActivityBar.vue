<template>
  <div class="activity-bar d-flex flex-column">
    <ul class="nav mt-auto">
      <li>
        <div class="icon d-flex align-items-center justify-content-center">
          <a
            href="https://github.com/tsukachu/tsukachu.github.io"
            target="_blank"
          >
            <font-awesome-icon :icon="['fab', 'github']" />
          </a>
        </div>
      </li>
    </ul>
  </div>
</template>

<style lang="scss">
.activity-bar {
  background-color: rgb(51, 51, 51);
  width: 48px;
}

.icon {
  height: 48px;
  width: 48px;

  margin-bottom: 4px;

  svg {
    font-size: 24px;
    color: rgba(255, 255, 255, 0.4);

    &:hover {
      color: rgb(255, 255, 255);
    }
  }
}
</style>
