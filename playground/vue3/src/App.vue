<script setup lang="ts">
import DefineRender from './examples/define-render/index.vue'
import DefineOptions from './examples/define-options/index.vue'
import DefineProps from './examples/define-props/index.vue'
import DefinePropsRefs from './examples/define-props-refs/index.vue'
import HoistStatic from './examples/hoist-static/index.vue'
import DefineModelReactivity from './examples/define-models/reactivity-transform/parent.vue'
import DefineModelRuntime from './examples/define-models/runtime/parent.vue'
import DefineSlots from './examples/define-slots/parent.vue'
import ExportProps from './examples/export-props/index.vue'
import ExportExpose from './examples/export-expose/index.vue'
import ExportRender from './examples/export-render/index.vue'
import BetterDefine from './examples/better-define/index.vue'
// import NamedTemplate from './examples/named-template/index.vue'
import SetupBlock from './examples/setup-block/index.vue'
import ChainCall from './examples/chain-call/index.vue'
import ReactivityTransform from './examples/reactivity-transform/index.vue'
import JsxDirective from './examples/jsx-directive/index.vue'
import BooleanProp from './examples/boolean-prop/index.vue'

import DefineProp from './examples/define-prop/index.vue'
import DefineEmit from './examples/define-emit/index.vue'

import { SetupComponentFoo } from './examples/setup-component'

import SetupSFC from './examples/setup-sfc/index.setup'
import ShortVmodel from './examples/short-vmodel/parent.vue'
import Full from './examples/full.setup'
</script>

<template>
  <div grid="~ cols-3 gap2">
    <fieldset>
      <legend>defineOptions</legend>
      <DefineOptions />
    </fieldset>

    <fieldset>
      <legend>defineRender</legend>
      <DefineRender />
    </fieldset>

    <fieldset>
      <legend>defineProps</legend>
      <DefineProps />
    </fieldset>

    <fieldset>
      <legend>definePropsRefs</legend>
      <DefinePropsRefs />
    </fieldset>

    <fieldset>
      <legend>exportProps</legend>
      <ExportProps />
    </fieldset>

    <fieldset>
      <legend>exportExpose</legend>
      <ExportExpose />
    </fieldset>

    <fieldset>
      <legend>hoistStatic</legend>
      <HoistStatic />
    </fieldset>

    <fieldset>
      <legend>namedTemplate</legend>
      <!-- <NamedTemplate /> -->
      TODO
    </fieldset>

    <fieldset>
      <legend>defineModels</legend>
      <DefineModelRuntime />
      <DefineModelReactivity />
    </fieldset>

    <fieldset>
      <legend>defineSlots</legend>
      <DefineSlots />
    </fieldset>

    <fieldset>
      <legend>betterDefine</legend>
      <BetterDefine />
    </fieldset>

    <fieldset>
      <legend>setupComponent</legend>
      <SetupComponentFoo />
    </fieldset>

    <fieldset>
      <legend>setupSFC</legend>
      <SetupSFC />
    </fieldset>

    <fieldset>
      <legend>setupBlock</legend>
      <SetupBlock />
    </fieldset>

    <fieldset>
      <legend>Short v-model</legend>
      <short-vmodel />
    </fieldset>

    <fieldset>
      <legend>Full example</legend>
      <Full model-value="123" />
    </fieldset>

    <fieldset>
      <legend>defineProp</legend>
      <DefineProp />
    </fieldset>

    <fieldset>
      <legend>defineEmit</legend>
      <DefineEmit />
    </fieldset>

    <fieldset>
      <legend>chainCall</legend>
      <ChainCall />
    </fieldset>

    <fieldset>
      <legend>reactivityTransform</legend>
      <ReactivityTransform />
    </fieldset>

    <fieldset>
      <legend>jsxDirective</legend>
      <JsxDirective />
    </fieldset>

    <fieldset>
      <legend>booleanProp</legend>
      <BooleanProp />
    </fieldset>

    <fieldset>
      <legend>exportRender</legend>
      <ExportRender />
    </fieldset>
  </div>
</template>

<style>
legend {
  font-family: monospace;
  font-size: 16px;
  font-weight: bold;
}

.ok {
  color: green;
}

.fail {
  font-weight: bold;
  color: red;
}

.ok,
.fail {
  padding: 10px;
}
</style>
