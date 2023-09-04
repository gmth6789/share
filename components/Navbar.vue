<template>
  <div>
  	
		<diy-navbar :isFixed="true" Header bgColor="pink">
			<template v-slot:content>
				<view Header style="height: 100%" class="flex align-center flex-nowrap diygw-col-24 items-start" @tap="navigateTo" data-type="page" data-url="/pages/index">
					<diy-navbar :isFixed="true" bgColor="pink" :isHome="true" :isBack="true">
						<!-- #ifndef VUE3 -->
						<block slot="backText"> กลับ </block>
						<block slot="content"> หน้าหลัก </block>
						<!-- #endif -->
						<!-- #ifdef VUE3 -->
						<template v-slot:backText> กลับ </template>
						<template v-slot:content> หน้าหลัก </template>
						<!-- #endif -->
					</diy-navbar>
				</view>
			</template>
		</diy-navbar>
  </div>
</template>
