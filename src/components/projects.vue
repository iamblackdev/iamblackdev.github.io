<template>
	<div>
		<div id="projects">
			<h2 class="section-header js-scroll-trigger sticky-top">Projects</h2>

			<a v-for="work in works" :key="work.name" target="_blank" :href="work.link">
				<div @mouseenter="projectEnter(work)" @mouseleave="projectLeave(work)" class="project-card" :class="{ projectCardHoverEffect: work.projectActive }">
					<p class="tech-used">
						{{ work.techUsed }}
					</p>
					<h3 class="project-title">
						{{ work.name }}
					</h3>
					<p class="project-description">
						{{ work.description }}
					</p>
					<div class="project-icons">
						<!-- GitHub -->
						<a v-if="work.github" target="_blank" :href="work.github">
							<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="icon">
								<path
									d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 
                   11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04
                   -3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 
                   3.633 17.7c-1.087-.744.084-.729.084-.729 
                   1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 
                   2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605
                   -2.665-.3-5.466-1.332-5.466-5.93 
                   0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 
                   0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 
                   3-.405 1.02.006 2.04.138 3 .405 
                   2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 
                   2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 
                   0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 
                   2.22 0 1.606-.015 2.896-.015 3.286 
                   0 .315.21.69.825.57C20.565 22.092 24 
                   17.592 24 12.297c0-6.627-5.373-12-12-12"
								></path>
							</svg>
						</a>

						<!-- iOS App Store -->
						<a v-if="work.ios" target="_blank" :href="work.ios">
							<svg viewBox="0 0 384 512" class="icon">
								<path
									d="M318.7 268.7c-.3-37.3 16.4-65.4 
                 50-86.1-18.8-26.9-47.2-41.7-84.9-44.6-35.7-2.8-74.4 
                 21.4-88.1 21.4-14.3 0-47.3-20.5-73.3-20-55.2.8-114.1 
                 44.5-114.1 133.4 0 28.3 5.2 57.7 15.6 87.3 
                 13.9 37.3 64.3 128.6 116.5 127 
                 27.3-.6 46.5-19.2 81.8-19.2 34.7 0 52.6 
                 19.2 83.3 19.2 53-.8 96.6-82.8 
                 110.2-120.4-70.3-26.5-66.3-101.6-67-118.1zM257 
                 78.1c27.4-32.4 24.9-61.9 24-72.1-24.1 
                 1.4-52 16.4-68.1 35.9-18.1 21.8-28.6 
                 48.5-26.4 76.2 26.1 2 50.8-11.3 70.5-40z"
								></path>
							</svg>
						</a>

						<!-- Android (Google Play) -->
						<a v-if="work.android" target="_blank" :href="work.android">
							<svg viewBox="0 0 512 512" class="icon">
								<path
									d="M325.3 234.3L104.6 5.9c-8.1-8.1-21.9-2.3-21.9 
                 9.1v482c0 11.4 13.8 17.2 21.9 
                 9.1l220.7-228.4c10.1-10.4 10.1-27.5 0-38.8zM361 
                 198.8l-29.3-30.3-45.1 46.7 45.1 
                 46.7 29.3-30.3c7.6-7.9 7.6-20.7 0-28.8zM361 
                 343.2l-29.3-30.3-45.1 46.7 45.1 
                 46.7 29.3-30.3c7.6-7.9 7.6-20.7 0-28.8z"
								></path>
							</svg>
						</a>
					</div>
				</div>
			</a>
		</div>
	</div>
</template>

<script>
import Json from '../../public/works.json';

export default {
	data() {
		return {
			works: Json,
		};
	},
	methods: {
		projectEnter(work) {
			this.works.forEach((e) => {
				e.projectActive = true;
			});
			work.projectActive = false;
		},
		projectLeave() {
			this.works.forEach((e) => {
				e.projectActive = false;
			});
		},
	},
};
</script>

<style>
#projects a:hover {
	text-decoration: none;
	color: inherit;
}
.project-card {
	padding: 40px;
	background-color: rgba(32, 32, 34, var(--bg-opacity));
	transition: all 0.3s ease;
	margin-bottom: 10px;
}
.project-card:hover {
	transform: scale(1.15);
}
.tech-used {
	font-size: 10px;
	font-weight: 700;
	letter-spacing: 3px;
	text-transform: uppercase;
	color: white;
}
.projectCardHoverEffect {
	opacity: 0.5;
}

.project-title {
	margin-top: 20px;
	line-height: 1.25px;
	font-size: 24px;
	font-weight: 600;
}

.project-description {
	margin-top: 20px;
	font-size: 14px;
	color: rgb(148, 148, 149);
}
.project-rating svg {
	color: rgb(148, 148, 149);
}
.rating-count {
	color: rgb(148, 148, 149);
	font-size: 10px;
	font-weight: 600;
	letter-spacing: 2px;
}

.project-icons {
	margin-top: 20px;
	display: flex;
	gap: 12px;
	align-items: center;
}

.icon {
	width: 18px;
	height: 18px;
	fill: white;
	opacity: 0.7;
	transition: 0.2s ease;
}

.icon:hover {
	opacity: 1;
	transform: scale(1.15);
}

@media (max-width: 991.98px) {
	.project-card:hover {
		transform: scale(1);
	}
	.projectCardHoverEffect {
		opacity: 1;
	}
}
@media (max-width: 767.98px) {
	.project-title {
		line-height: 30px;
	}
}
</style>
