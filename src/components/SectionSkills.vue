/*
 * Created on Tue Mar 31 2020 by Johnathan Irvin
 *
 * This program is free software: you can redistribute it and/or modify
 * it under the terms of the GNU General Public License as published by
 * the Free Software Foundation, either version 3 of the License, or
 * (at your option) any later version.
 *
 * This program is distributed in the hope that it will be useful,
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 */

<template lang="pug">
  BaseSection#skills.container
    h2.text-center.p-2.h1.text-center.d-none Skills
    .flex.text-center.icons.align-center
      i.devicon-css3-plain-wordmark.colored.icon
      i.devicon-html5-plain-wordmark.colored.icon
      i.devicon-javascript-plain.colored.icon
      i.devicon-bootstrap-plain.colored.icon
      i.devicon-jquery-plain-wordmark.colored.icon
      i.devicon-nodejs-plain-wordmark.colored.icon
      i.devicon-vuejs-plain-wordmark.colored.icon
      i.devicon-python-plain-wordmark.colored.icon
      i.devicon-csharp-plain-wordmark.colored.icon
      i.devicon-confluence-plain-wordmark.colored.icon
      i.devicon-docker-plain-wordmark.colored.icon
      i.devicon-git-plain-wordmark.colored.icon
</template>

<script>
import 'devicon';
import BaseSection from '@/components/BaseSection';

export default {
  name: 'TheSectionSkills',
  components: {
    BaseSection
  },
};
</script>

<style lang="scss">
#skills {
  position: relative;

  .align-center {
    display: flex;
    align-content: space-evenly;
    justify-content: space-around;
  }

  .icons {
    font-size: 0.9rem;
    z-index: 100;
    position: relative;
    min-width: 100%;
    height: 100%;
    min-height: 100%;
  }
}
</style>

<style scoped>
.flex {
  display: flex;
  align-content: center;
  justify-content: space-around;
  flex-wrap: wrap;
  padding: 10px;
}

.icon::before {
  font-size: 6em;
}

.icon {
  margin: 10px;
  min-width: 20%;
}
</style>
